# my-images-sync
> fork 这个仓库, 创建你自己的docker register 账号密码:

- Settings
- Secrets
- New Repository Secrets
- Add your DOCKER_USERNAME and DOCKER_PASSWORD key values.

> 修改images.json 文件，改成你需要的
~~~powershell
{
  "quay.io/coreos/kube-rbac-proxy": "minyi/kube-rbac-proxy",
  "k8s.gcr.io/metrics-server/metrics-server": "minyi/metrics-server",
  "k8s.gcr.io/ingress-nginx/controller": "minyi/ingress-nginx-controller",
  "k8s.gcr.io/git-sync/git-sync": "minyi/git-sync",
  "k8s.gcr.io/kube-state-metrics/kube-state-metrics": "minyi/kube-state-metrics",
  "k8s.gcr.io/sig-storage/nfs-subdir-external-provisioner": "minyi/nfs-subdir-external-provisioner",
  "k8s.gcr.io/prometheus-adapter/prometheus-adapter": "minyi/prometheus-adapter",
  "k8s.gcr.io/kube-apiserver": "minyi/kube-apiserver",
  "k8s.gcr.io/kube-controller-manager": "minyi/kube-controller-manager",
  "k8s.gcr.io/kube-scheduler": "minyi/kube-scheduler",
  "k8s.gcr.io/kube-proxy": "minyi/kube-proxy",
  "k8s.gcr.io/pause": "minyi/pause",
  "k8s.gcr.io/etcd": "minyi/etcd",
  "k8s.gcr.io/coredns/coredns": "minyi/coredns",
  "k8s.gcr.io/ingress-nginx/kube-webhook-certgen": "minyi/kube-webhook-certgen",
  "k8s.gcr.io/ingress-nginx/opentelemetry": "minyi/opentelemetry",
  "k8s.gcr.io/defaultbackend-amd64": "minyi/defaultbackend-amd64"
}
~~~

> 修改auth.json，可以添加其他 docker register源
~~~powershell
{
  "registry.hub.docker.com": {
    "username": "${DOCKER_USERNAME}",
    "password": "${DOCKER_PASSWORD}"
  }
}
~~~