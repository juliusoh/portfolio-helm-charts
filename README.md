helm upgrade portfolio portfolio --install --values=portfolio/values.yaml --namespace=portfolio --create-namespace

helm install aws-load-balancer-controller eks/aws-load-balancer-controller -n kube-system --set clusterName=tf-juliusoh-eks-cluster-us-west-2 --set serviceAccount.create=false --set serviceAccount.name-=aws-load-balancer-controller

