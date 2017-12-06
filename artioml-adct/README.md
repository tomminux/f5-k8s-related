# Deployment of ArtiomL ADCT on Kubernetes cluster
This projetc collects some example files to correctly deploy the ADCT Container managed my ArtiomL: [ArtiomL ADCT Project on GitHub](https://github.com/ArtiomL/adct) in a Kubernetes Cluster

* [adct-services.yaml](https://github.com/tomminux/f5-k8s-related/blob/master/artioml-adct/adct-services.yml) will deploy services needed to publish port 80 and port 443 on the cluster
* [adct-deployment.yaml](https://github.com/tomminux/f5-k8s-related/blob/master/artioml-adct/adct-deployment.yml) will deploy PODs using [arioml/adct container](https://hub.docker.com/r/artioml/adct/)
* [adct-http-configMap.yaml.yaml](https://github.com/tomminux/f5-k8s-related/blob/master/artioml-adct/adct-http-configMap.yml) will create a configmap containig instruction on how to provision the HTTP service for this applicaiton on a BIG-IP ADC (north-south traffic management)
* [adct-https-configMap.yaml.yaml](https://github.com/tomminux/f5-k8s-related/blob/master/artioml-adct/adct-https-configMap.yml) will create a configmap containig instruction on how to provision the HTTPS service for this applicaiton on a BIG-IP ADC (north-south traffic management)

