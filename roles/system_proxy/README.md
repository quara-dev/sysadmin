# Role variables

| Name                 |                              Default/Required                               | Description                            |
| -------------------- | :-------------------------------------------------------------------------: | -------------------------------------- |
| `system_http_proxy`  |                        `"http://10.100.100.1:3128"`                         | Address of HTTP proxy                  |
| `system_https_proxy` |                        `"http://10.100.100.1:3128"`                         | Address of HTTPS proxy                 |
| `system_no_proxy`    | `"localhost,127.0.0.1,quara.azurecr.io,azure.dev,azure.com,10.18.164.0/16"` | Proxy will not be used for those hosts |
| `system_ftp_proxy`   |                                   `unset`                                   | Address of FTP proxy                   |
