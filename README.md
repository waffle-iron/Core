[![Stories in Ready](https://badge.waffle.io/VATSIM-UK/core.png?label=ready&title=Ready)](https://waffle.io/VATSIM-UK/core)
[![Stories in Ready](https://badge.waffle.io/cloud10-ide/core.png?label=ready&title=Ready)](https://waffle.io/cloud10-ide/core)
# [Cloud10](https://cloud10-ide.github.io/)

This is a fork of Cloud9 meant as a self-hosted cloud IDE. 

## Installation

Follow these steps to install Cloud10:

    git clone https://github.com/cloud10-ide/core.git
    cd cloud10
    scripts/install-sdk.sh
    
To update the SDK to the latest version run:

    git pull origin master
    scripts/install-sdk.sh

### Starting Cloud10

Start Cloud10 as follows:

    node server.js

The following options can be used:

    --settings       Settings file to use
    --help           Show command line options.
    -t               Start in test mode
    -k               Kill tmux server in test mode
    -b               Start the bridge server - to receive commands from the cli  [default: false]
    -w               Workspace directory
    --port           Port
    --debug          Turn debugging on
    --listen         IP address of the server
    --readonly       Run in read only mode
    --packed         Whether to use the packed version.
    --auth           Basic Auth username:password
    --collab         Whether to enable collab.
    --no-cache       Don't use the cached version of CSS

Now visit [http://localhost:8181/ide.html](http://localhost:8181/ide.html) to load Cloud9.

### Running Tests

Run server side tests with:

    npm run test

Run client side tests with:

    npm run ctest

Then visit [http://localhost:8181/static/test](http://localhost:8181/static/test) in your browser.

## To Do

- [ ] Fully rename it to Cloud10
- [ ] Make it production-ready
- [ ] Make a GUI for managing workspaces
