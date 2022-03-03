# Petio
Homepages: [petio](https://github.com/petio-team/petio) 

**Petio** Allow your users to interact with media both on and off your server with this app. Available as a docker image and also as binaries. Features a React frontend utilizing Redux and a Node JS express API and MongoDb database.

## Usage

Set `petio_enabled: true` in your `/inventories/[my inventory]/group_vars/nas.yml` file.

The Prowlarr web interface can be found at `http://ansible_nas_host_or_ip:7777` by default