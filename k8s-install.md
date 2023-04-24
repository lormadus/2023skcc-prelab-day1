## eksctl 설치
```
curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
```

## kubectl 설치
```
curl -O https://s3.us-west-2.amazonaws.com/amazon-eks/1.25.7/2023-03-17/bin/linux/amd64/kubectl
```

## K8s 클러스터 설치 (Region Code 수정)
```
eksctl create cluster --nodes-min=2 --nodes-max=3 --name my-cluster --region eu-north-1 --nodes=2
```

## Sample App
https://github.com/aws-containers/retail-store-sample-app
