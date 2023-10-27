# ansible_compose

**Before using this role, I highly recommend to read README.md in [compose-collection repository](https://github.com/vdbogdanov/compose-collection)!**

| Task     | Description      		                                   |
| -------- | --------------------------------------------------------- |
| openvpn  | Deploy OpenVPN and generate .ovpn config on your machine. |
| nginx    | Deploy Nginx as reverse proxy with HTTPS protocol.        |
| gitlab   | Deploy Gitlab service.                                    |
| cmdbuild | Deploy CMDBuild base                                      |
| pgadmin  | Deploy pgAdmin service.                                   |
| vcenter  | Deploy vcsim - vcenter simulator.                         |

For using this role, you should copy compose-collection on your server:

```
ansible-playbook -i inventories/example site.yaml -t "compose_config, copy_compose_collection"
```

To change the standard configuration of services, you can use [roles/compose_config/defaults/main.yaml](roles/compose_config/defaults/main.yaml).