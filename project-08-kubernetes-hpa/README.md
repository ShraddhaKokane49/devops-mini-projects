# Kubernetes Horizontal Pod Autoscaler (HPA)

## Objective

Automatically scale pods based on CPU utilization.

## Commands Used

Create deployment:

kubectl create deployment php-apache --image=k8s.gcr.io/hpa-example

Expose deployment:

kubectl expose deployment php-apache --port=80

Create HPA:

kubectl autoscale deployment php-apache --cpu-percent=50 --min=1 --max=5

Check HPA:

kubectl get hpa

## Outcome

Kubernetes automatically increases or decreases pods based on CPU load.