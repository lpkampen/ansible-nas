
# Code Server

Homepage: [https://github.com/linuxserver/docker-code-server](https://github.com/linuxserver/docker-code-server)

Code-server is VS Code running on a remote server, accessible through the browser.

## Usage

Set `code_server_enabled: true` in your `inventories/<your_inventory>/nas.yml` file.

The Code Server web interface can be found at http://ansible_nas_host_or_ip:8443.


## Specific Configuration

Remember to add passwords to your `inventories/<your_inventory>/nas.yml` file.
If you want to use hashed passwords, then look at the devs docs, unless you got the knowledge yourself of course.

code_server_password: "password" 
# code_server_hashed_password: ""
code_server_sudo_password: "sudopassword"
# code_server_sudo_password_hash: ""

I`ve also added two folders to the container, to mount project folders, add these lines and fill in the right info for you, examples:

code_server_mount_directory: "{{ docker_home }}"
code_server_code_directory: " /codefolder "
