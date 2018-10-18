# cryptoping | README

* NOTE -- we use docker compose v2 files due to hyper.sh constraints

## Setup
This repository include submodules, to get them to a working state execute:

    git submodule init && git submodule update

Then traverse into the respective submodules to check out the correct branches:

    git checkout <branch>

If you make changes to the submodules, you'll also want to add them to a commit
for `cryptoping` so that the hash is recorded.

NOTE: in the docker compose files we use `links` over `networks` due to the ultimate deploy endpoint (`hyper.sh`)
