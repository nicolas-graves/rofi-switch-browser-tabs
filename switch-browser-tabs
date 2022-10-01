#!/usr/bin/env bash

TABS_JSON=$(wget -q -O- http://localhost:9222/json/list | sed -e "s/^'//" -e "s/'$//" | jq -r 'map(select(.type == "page") | {id: .id, title: .title})')

if [[ -z $@ ]]; then
    TAB_NAMES=$(echo "$TABS_JSON" | jq -r 'map(.title) | .[]')

    echo "$TAB_NAMES"
else
    TAB=$*

    TAB_ID=$(echo "$TABS_JSON" | jq -r "map(select(.title | contains (\"${TAB//\"/\\\"}\")) | .id) | .[]")

    $(wget -q -O- http://localhost:9222/json/activate/$TAB_ID >/dev/null)
fi
