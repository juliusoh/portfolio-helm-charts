helm upgrade portfolio portfolio --install --values=portfolio/values.yaml --namespace=portfolio --create-namespace

helm upgrade point-of-sale point-of-sale --install --values=point-of-sale/values.yaml --namespace=point-of-sale --create-namespace

helm upgrade ecommerce ecommerce --install --values=ecommerce/values.yaml --namespace=ecommerce --create-namespace

helm install aws-load-balancer-controller eks/aws-load-balancer-controller -n kube-system --set clusterName=tf-juliusoh-eks-cluster-us-west-2 --set serviceAccount.create=false --set serviceAccount.name-=aws-load-balancer-controller

https://github.com/jetstack/cert-manager/releases/download/v1.5.3/cert-manager.yaml

