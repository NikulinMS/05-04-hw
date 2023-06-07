# Домашнее задание к занятию "`Оркестрация группой Docker-контейнеров на примере Docker Compose`" - `Никулин Михаил Сергеевич`



---

### Задание 1

![task_1_1.png](img%2Ftask_1_1.png)
![task_1_2.png](img%2Ftask_1_2.png)

---

### Задание 2


```
root@nikulin:~/test# terraform apply

Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following symbols:
  + create

Terraform will perform the following actions:

  # yandex_compute_instance.node01 will be created
  + resource "yandex_compute_instance" "node01" {
      + allow_stopping_for_update = true
      + created_at                = (known after apply)
      + folder_id                 = (known after apply)
      + fqdn                      = (known after apply)
      + gpu_cluster_id            = (known after apply)
      + hostname                  = "node01.netology.cloud"
      + id                        = (known after apply)
      + metadata                  = {
          + "ssh-keys" = <<-EOT
                centos:ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQC+iKSOjHPJFf5+8iaOjmzIkDfo0AqCfbmQRM4YMtM6Hwb8H9A5DbYPmiqWsXh7wqnMxL5eClgpOGvM2Rmjqxrz5hVcU6KOAtiLk1Hv/Sd56yj7FrP8OAf+WDS/02wnu7kIRH+5iU2kEBhlmRYixsNGiCTIFBldpgZUXY87ML9Z38CGVSX7Y/TPpixQlQjKVhXa0+NwhgbLYo7M9klspUpZ8gTGOpv39rb+Kgp/YlyDi/KHi5Fu3fVUReaMRAppHzHr7FxI57B0Fx90YElUdbJjZhduwFhfzqktWtiqJFCHh3Wzcgdk8ohvyS/rCJaPPIwp/+kl+rytPed0lKP1c1xVXoREZInGXlvNMjyZAlUQnH4/OWDrAHu6FwT36kD5RQ1eIMVmqa1cOk2hXT33NKjfyfPosTp3iwkjUznVVPCEqVHRpMx6/49Ko6PLWRrKN0aEsKY/aLVfdQ4McvL8N9W2Wbm4x7ifC3e3GB/25DS4QueIa53WJF+gzj6nQIRoet0= root@nikulin
            EOT
        }
      + name                      = "node01"
      + network_acceleration_type = "standard"
      + platform_id               = "standard-v1"
      + service_account_id        = (known after apply)
      + status                    = (known after apply)
      + zone                      = "ru-central1-a"

      + boot_disk {
          + auto_delete = true
          + device_name = (known after apply)
          + disk_id     = (known after apply)
          + mode        = (known after apply)

          + initialize_params {
              + block_size  = (known after apply)
              + description = (known after apply)
              + image_id    = "fd8eimjigan6lhc2v4g5"
              + name        = "root-node01"
              + size        = 50
              + snapshot_id = (known after apply)
              + type        = "network-nvme"
            }
        }

      + metadata_options {
          + aws_v1_http_endpoint = (known after apply)
          + aws_v1_http_token    = (known after apply)
          + gce_http_endpoint    = (known after apply)
          + gce_http_token       = (known after apply)
        }

      + network_interface {
          + index              = (known after apply)
          + ip_address         = (known after apply)
          + ipv4               = true
          + ipv6               = (known after apply)
          + ipv6_address       = (known after apply)
          + mac_address        = (known after apply)
          + nat                = true
          + nat_ip_address     = (known after apply)
          + nat_ip_version     = (known after apply)
          + security_group_ids = (known after apply)
          + subnet_id          = (known after apply)
        }

      + placement_policy {
          + host_affinity_rules = (known after apply)
          + placement_group_id  = (known after apply)
        }

      + resources {
          + core_fraction = 100
          + cores         = 8
          + memory        = 8
        }

      + scheduling_policy {
          + preemptible = (known after apply)
        }
    }

  # yandex_vpc_network.default will be created
  + resource "yandex_vpc_network" "default" {
      + created_at                = (known after apply)
      + default_security_group_id = (known after apply)
      + folder_id                 = (known after apply)
      + id                        = (known after apply)
      + labels                    = (known after apply)
      + name                      = "net"
      + subnet_ids                = (known after apply)
    }

  # yandex_vpc_subnet.default will be created
  + resource "yandex_vpc_subnet" "default" {
      + created_at     = (known after apply)
      + folder_id      = (known after apply)
      + id             = (known after apply)
      + labels         = (known after apply)
      + name           = "subnet"
      + network_id     = (known after apply)
      + v4_cidr_blocks = [
          + "192.168.101.0/24",
        ]
      + v6_cidr_blocks = (known after apply)
      + zone           = "ru-central1-a"
    }

Plan: 3 to add, 0 to change, 0 to destroy.

Changes to Outputs:
  + external_ip_address_node01_yandex_cloud = (known after apply)
  + internal_ip_address_node01_yandex_cloud = (known after apply)

Do you want to perform these actions?
  Terraform will perform the actions described above.
  Only 'yes' will be accepted to approve.

  Enter a value: yes
```

![task_2_1.png](img%2Ftask_2_1.png)
![task_2_2.png](img%2Ftask_2_2.png)

---

### Задание 3

![task_3_1.png](img%2Ftask_3_1.png)
![task_3_2.png](img%2Ftask_3_2.png)
---

### Задание 4

![task_4_1.png](img%2Ftask_4_1.png)

---
## Дополнительные задания (со звездочкой*)


### Задание 5

![task_5_1.png](img%2Ftask_5_1.png)
![task_5_2.png](img%2Ftask_5_2.png)
![task_5_3.png](img%2Ftask_5_3.png)
![task_5_4.png](img%2Ftask_5_4.png)