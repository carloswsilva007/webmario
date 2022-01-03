# webmario
Projeto_Webmario_Terraform
.terraform/plugins/linux_amd64/lock.json

.terraform/plugins/linux_amd64/terraform-provider-docker_v2.7.2_x4

# Baixar a imagem do Projeto Docker-SuperMario
resource "docker_image" "image_id" {
  name = "pengbai/docker-supermario:latest"
}

# Inicia o Container
resource "docker_container" "container_id" {
  name  = "supermario"
  image = "${docker_image.image_id.latest}"
  ports {
    internal = "8080"
    external = "80"
  }
}

main.ti

terraform.tfstate

@@ -0,0 +1,122 @@
{
  "version": 4,
  "terraform_version": "0.12.7",
  "serial": 5,
  "lineage": "88753f55-ca6b-1b9d-610f-8fff2794e7ab",
  "outputs": {},
  "resources": [
    {
      "mode": "managed",
      "type": "docker_container",
      "name": "container_id",
      "provider": "provider.docker",
      "instances": [
        {
          "schema_version": 2,
          "attributes": {
            "attach": false,
            "bridge": "",
            "capabilities": [],
            "command": [
              "catalina.sh",
              "run"
            ],
            "container_logs": null,
            "cpu_set": "",
            "cpu_shares": 0,
            "destroy_grace_seconds": null,
            "devices": [],
            "dns": [],
            "dns_opts": [],
            "dns_search": null,
            "domainname": "",
            "entrypoint": [],
            "env": null,
            "exit_code": null,
            "gateway": "172.17.0.1",
            "group_add": null,
            "healthcheck": [],
            "host": [],
            "hostname": "fe02733aaf95",
            "id": "fe02733aaf95a1bbb49da69a03b7cf347abb048c18b8fde8dc5dda1cf66d4f1e",
            "image": "sha256:077ed8c9236afe7875e1678f17150b9f1bf2691fde6c4b81b0253695ec627bbc",
            "ip_address": "172.17.0.2",
            "ip_prefix_length": 16,
            "ipc_mode": "private",
            "labels": [],
            "links": null,
            "log_driver": "json-file",
            "log_opts": {},
            "logs": false,
            "max_retry_count": 0,
            "memory": 0,
            "memory_swap": 0,
            "mounts": [],
            "must_run": true,
            "name": "supermario",
            "network_alias": null,
            "network_data": [
              {
                "gateway": "172.17.0.1",
                "ip_address": "172.17.0.2",
                "ip_prefix_length": 16,
                "network_name": "bridge"
              }
            ],
            "network_mode": "default",
            "networks": null,
            "networks_advanced": [],
            "pid_mode": "",
            "ports": [
              {
                "external": 80,
                "internal": 8080,
                "ip": "0.0.0.0",
                "protocol": "tcp"
              }
            ],
            "privileged": false,
            "publish_all_ports": false,
            "read_only": false,
            "restart": "no",
            "rm": false,
            "shm_size": 64,
            "start": true,
            "sysctls": null,
            "tmpfs": null,
            "ulimit": [],
            "upload": [],
            "user": "mario",
            "userns_mode": "",
            "volumes": [],
            "working_dir": "/usr/local/tomcat"
          },
          "private": "eyJzY2hlbWFfdmVyc2lvbiI6IjIifQ==",
          "depends_on": [
            "docker_image.image_id"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "docker_image",
      "name": "image_id",
      "provider": "provider.docker",
      "instances": [
        {
          "schema_version": 0,
          "attributes": {
            "id": "sha256:077ed8c9236afe7875e1678f17150b9f1bf2691fde6c4b81b0253695ec627bbcpengbai/docker-supermario:latest",
            "keep_locally": null,
            "latest": "sha256:077ed8c9236afe7875e1678f17150b9f1bf2691fde6c4b81b0253695ec627bbc",
            "name": "pengbai/docker-supermario:latest",
            "pull_trigger": null,
            "pull_triggers": null
          },
          "private": "bnVsbA=="
        }
      ]
    }
  ]
}

terraform.tfstate.backup

@@ -0,0 +1,122 @@
{
  "version": 4,
  "terraform_version": "0.12.7",
  "serial": 3,
  "lineage": "88753f55-ca6b-1b9d-610f-8fff2794e7ab",
  "outputs": {},
  "resources": [
    {
      "mode": "managed",
      "type": "docker_container",
      "name": "container_id",
      "provider": "provider.docker",
      "instances": [
        {
          "schema_version": 2,
          "attributes": {
            "attach": false,
            "bridge": "",
            "capabilities": [],
            "command": [
              "catalina.sh",
              "run"
            ],
            "container_logs": null,
            "cpu_set": "",
            "cpu_shares": 0,
            "destroy_grace_seconds": null,
            "devices": [],
            "dns": [],
            "dns_opts": [],
            "dns_search": null,
            "domainname": "",
            "entrypoint": [],
            "env": null,
            "exit_code": null,
            "gateway": "172.17.0.1",
            "group_add": null,
            "healthcheck": [],
            "host": [],
            "hostname": "5eb93a423cdd",
            "id": "5eb93a423cdd648dc78a693affd8fbcdf2eaaad9248be6e425dbd680aa9fb644",
            "image": "sha256:077ed8c9236afe7875e1678f17150b9f1bf2691fde6c4b81b0253695ec627bbc",
            "ip_address": "172.17.0.2",
            "ip_prefix_length": 16,
            "ipc_mode": "private",
            "labels": [],
            "links": null,
            "log_driver": "json-file",
            "log_opts": {},
            "logs": false,
            "max_retry_count": 0,
            "memory": 0,
            "memory_swap": 0,
            "mounts": [],
            "must_run": true,
            "name": "supermario",
            "network_alias": null,
            "network_data": [
              {
                "gateway": "172.17.0.1",
                "ip_address": "172.17.0.2",
                "ip_prefix_length": 16,
                "network_name": "bridge"
              }
            ],
            "network_mode": "default",
            "networks": null,
            "networks_advanced": [],
            "pid_mode": "",
            "ports": [
              {
                "external": 70,
                "internal": 3000,
                "ip": "0.0.0.0",
                "protocol": "tcp"
              }
            ],
            "privileged": false,
            "publish_all_ports": false,
            "read_only": false,
            "restart": "no",
            "rm": false,
            "shm_size": 64,
            "start": true,
            "sysctls": null,
            "tmpfs": null,
            "ulimit": [],
            "upload": [],
            "user": "mario",
            "userns_mode": "",
            "volumes": [],
            "working_dir": "/usr/local/tomcat"
          },
          "private": "eyJzY2hlbWFfdmVyc2lvbiI6IjIifQ==",
          "depends_on": [
            "docker_image.image_id"
          ]
        }
      ]
    },
    {
      "mode": "managed",
      "type": "docker_image",
      "name": "image_id",
      "provider": "provider.docker",
      "instances": [
        {
          "schema_version": 0,
          "attributes": {
            "id": "sha256:077ed8c9236afe7875e1678f17150b9f1bf2691fde6c4b81b0253695ec627bbcpengbai/docker-supermario:latest",
            "keep_locally": null,
            "latest": "sha256:077ed8c9236afe7875e1678f17150b9f1bf2691fde6c4b81b0253695ec627bbc",
            "name": "pengbai/docker-supermario:latest",
            "pull_trigger": null,
            "pull_triggers": null
          },
          "private": "bnVsbA=="
        }
      ]
    }
  ]
}
