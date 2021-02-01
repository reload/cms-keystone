# Install postgresql on MacOS

* Install with Homebrew: `brew install postgres`

Setup a launchagent and start it
* `mkdir -p ~/Library/LaunchAgents`
* `ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents`
* `launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist`

Create a database (call it Grayskull for no reason)
createdb grayskull

In the project directory run the following:
* `yarn install`
* `yarn create-tables`
* `yarn dev`
