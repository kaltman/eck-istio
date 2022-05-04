# eck-istio
## Steps to reproduce

- istioctl install --set profile=demo -y, see [https://istio.io/latest/docs/setup/getting-started/](https://istio.io/latest/docs/setup/getting-started/)
- Install ECK operator with sidecar enabled as per this doc, [https://www.elastic.co/guide/en/cloud-on-k8s/current/k8s-service-mesh-istio.html](https://www.elastic.co/guide/en/cloud-on-k8s/current/k8s-service-mesh-istio.html)
- Install ECK manifest / ES & Kibana
- Apply ingress (http, https still not working)
- Check the ingress IP (kubectl get svc -n istio-ingress) and ajust your DNS entry (in my case, *.eck.kaltman.co)
