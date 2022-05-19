VERSION 0.6

IMPORT github.com/defn/cloud/lib:master AS lib

FROM lib+platform

update:
    COPY pyproject.toml poetry.lock .
    RUN ~/bin/e poetry update
    SAVE ARTIFACT poetry.lock
