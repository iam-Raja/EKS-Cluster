# EKS-CLUSTER & KUBECTL SET UP


**Steps:**

**Eks installation**
* Create & Manage Eks cluster

```
curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
```

```
sudo mv /tmp/eksctl /usr/local/bin
```

```
eksctl version
```
**Kubectl Setup:**
* Manage containers inside cluster

```
curl -O https://s3.us-west-2.amazonaws.com/amazon-eks/1.30.0/2024-05-12/bin/linux/amd64/kubectl
```

```
chmod +x ./kubectl
```

```
sudo mv kubectl /usr/local/bin/
```

```
kubectl version --client
```

**AWS Confugure**
* configure with access & secret key or with IAM roles
