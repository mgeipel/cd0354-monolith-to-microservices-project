# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline

I used GitHub Actions for the deployment pipeline. The screenshots below show the successful deployment of the application.

* DockerHub showing containers that you have pushed

![DockerHub](DockerHub.png)

* GitHub repository action logs

![CI/CD Logs](CICDlogs-online.png)

* Github Actions in VSCode

![CI/CD Logs](CICDlogs.png)


## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```

![Kubernetes Pods](Pods.png)

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```

![Kubernetes Services](Services.png)


* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```

![Kubernetes HPA](HPA.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```

![Kubernetes Logs](PodLogs.png)
