# Uptime Kuma

Monitoring Solution

## Sources

https://github.com/louislam/uptime-kuma

**Techno Tim Youtube**
https://www.youtube.com/watch?v=r_A5NKkAqZM


## Install with Argo CD

Use a central repository which links to all Apps which has to be deployed,
and add the App desciption there, or deploy the App for Uptime Kuma manually.
Find a sample in my [App of Apps Repo](https://github.com/wep4you/k8s-apps.git),
there is also a sample definition for [Uptime Kuma](https://github.com/wep4you/k8s-apps/blob/main/local/uptime-kuma.yml)

## Install manual with kubectl

To add your own configuration, copy ```overlays/local``` to a new folder and change the files to your needs.
It's standard Kustomize format you can use.

    ```
    kubectl apply -k overlays/local
    ```

# Troubleshooting

## ERR_SOCKET_BAD_PORT

Change ServiceName from **uptime-kuma** to something different like uptime-kuma-web

https://issueexplorer.com/issue/louislam/uptime-kuma/741
