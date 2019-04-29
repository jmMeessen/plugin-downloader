# Jenkins plugin and dependency downloader

This is based on the utility used to download plugins in a Jenkins Docker image

## Usage

Change directory to this directory.

Source the setup_env.sh script: `. ./setup_env.sh`

Then execute the `plugins.sh` script. The downloaded plugins will be available in the `./plugins/` directory.

### Download a plugin

`./plugins.sh mailer` to download the mailer plugin and its dependencies

### Download multiple plugins

`./plugins.sh mailer git-client` to download both plugins and their dependencies.

### Download a list of plugins

`./plugins.sh < plugins.txt` will process the list.

### To specify a given version

`./plugins.sh mailer:1.23`
