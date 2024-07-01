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
* create a yaml file and login workstation & clone yaml
```
eksctl create cluster --config-file=eks.yaml
```
* Deleting cluster
```
eksctl delete cluster --config-file=eks.yaml
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


**Namespace-Setup**

```
sudo git clone https://github.com/ahmetb/kubectx /opt/kubectx
```

```
sudo ln -s /opt/kubectx/kubens /usr/local/bin/kubens
```

* Give required ns-name 
```
kubens <ns-name>
```
