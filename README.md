# DO380 – OpenShift Labs

![OpenShift](https://img.shields.io/badge/OpenShift-EE0000?logo=redhatopenshift&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white) ![Apache](https://img.shields.io/badge/Apache_httpd-D22128?logo=apache&logoColor=white)

> OpenShift lab manifests (Pod, Deployment, Service) used while studying Red Hat DO380.

## Overview

Practice manifests for **Red Hat OpenShift**: a Pod and a Deployment running httpd from the cluster's internal image registry (CRC), exposed through a ClusterIP Service.

## Tech Stack

- **OpenShift**
- **Kubernetes**
- **Apache httpd**

## Repository Structure

```text
myapp/deployment-myapp.yml
myapp/pod.yml
myapp/svc-myapp.yml
README.md
```

## Getting Started

```bash
git clone https://github.com/Gamal-Mohammad/do380.git
cd do380
```

### Deploy to OpenShift

| File | Kind | Name |
|---|---|---|
| `myapp/deployment-myapp.yml` | Deployment | `myapp` |
| `myapp/pod.yml` | Pod | `pod1` |
| `myapp/svc-myapp.yml` | Service | `my-svc` |

```bash
oc apply -f myapp/deployment-myapp.yml
oc apply -f myapp/pod.yml
oc apply -f myapp/svc-myapp.yml
oc get pods,svc
```

## Author

**Gamal Mohammad**

[![GitHub](https://img.shields.io/badge/GitHub-Gamal--Mohammad-181717?logo=github)](https://github.com/Gamal-Mohammad)
