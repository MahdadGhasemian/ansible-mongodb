# Ansible Role: Mongodb Replecaset

Ansible galaxy role used to run a mongodb replecaset on a docker container

## Requirements

None.

## Role Variables
```yaml
docker_mongodb__name: mongodb
docker_mongodb__image: docker.io/bitnami/mongodb:latest
docker_mongodb__root_password: "pass1234"
docker_mongodb__replecaset_key: "replicasetkey"
docker_mongodb__replecaset_name: "replecaset"
docker_mongodb__first_user_username: "init_user"
docker_mongodb__first_user_password: "pass1234"
docker_mongodb__first_user_database_name: "init_database"
docker_mongodb__home: "/root/mongodb"
docker_mongodb__pull_image: yes
docker_mongodb__remove_existing_container: yes
docker_mongodb__port: 27030
docker_mongodb__network_name: "mongodb-network"
```

## Dependencies

- community.docker

## Example Playbook (using default package)

    - hosts: servers
      roles:
        - role: MahdadGhasemian.ansible-mongodb

## License

MIT / BSD

## Author Information

This role was created in 2023 by [Mahdad Ghasemian](https://mahdad.me/).