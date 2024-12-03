# Certificate secured Gateway API

## Purpose of this directory

This directory contains the manifest and terraform files to follow the blogpost

"Deploy an infrastructure stack on AWS that provides certificate-based encryption, based on Cert-Manager, Kubernetes Gateway API, and External-DNS" Link: TBD

## Subdirectories

```bash
.
├── README.md
├── manifests
│   ├── application                         # Contains the manifest files for the test application that will make use of the certificate secured Gateway API resource
│   │   ├── Deployment.yaml
│   │   └── Service.yaml
│   ├── gateway-api                         # Contains the manifest files for the Gateway API resources
│   │   ├── ClusterIssuer.yaml
│   │   ├── Gateway.yaml
│   │   └── HTTPRoute.yaml
│   └── iam                                 # Contains the AWS IAM policy definition file for the IAM role that will be linked to the External-DNS service account
│       └── ExternalDNS_permissions.json
└── terraform                               # Contains the Terraform files to deploy a testcluster to AWS
    ├── README.md
    ├── main.tf
    ├── outputs.tf
    ├── terraform.tf
    └── variables.tf
```
