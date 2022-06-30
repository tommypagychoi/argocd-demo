# argocd-demo
ArgoDC Demo
└── /resources
    ├── /base # 기본 manifest 리소스 
    │   ├── deployment.yaml
    │   └── service.yaml
    │
    ├── /helm # helm chart를 사용한 manifest 리소스
    │   ├── /templates
    │   │   ├── deployment.yaml
    │   │   └── service.yaml
    │   ├── Chart.yaml
    │   └── values.yaml
    │
    └── /helm-rollout # helm chart 및 Argo Rollouts를 사용한 manifest 리소스
        ├── /templates
        │   ├── rollout.yaml
        │   ├── service-active.yaml # Blue 전용 service 
        │   └── service-preview.yaml # Green 전용 service 
        ├── Chart.yaml
        └── values.yaml
