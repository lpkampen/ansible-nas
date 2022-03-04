# Petio
Homepages: [petio](https://github.com/petio-team/petio) 

**Petio** Allow your users to interact with media both on and off your server with this app. Available as a docker image and also as binaries. Features a React frontend utilizing Redux and a Node JS express API and MongoDb database.

## Usage

Set `petio_enabled: true` in your `/inventories/[my inventory]/group_vars/nas.yml` file.

The Petio web interface can be found at `http://ansible_nas_host_or_ip:27777` by default

## Specific Configuration

When setting up the web interface, you will have to add the mongo database, for now you have to add it manualy: ansible_ip:27017