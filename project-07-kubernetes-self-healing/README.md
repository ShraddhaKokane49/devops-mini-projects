# Kubernetes Self-Healing Demo

## Objective
Demonstrate Kubernetes self-healing using a Deployment with 3 replicas.

## Commands Used

Create deployment:

kubectl create deployment nginx-demo --image=nginx

Scale deployment:

kubectl scale deployment nginx-demo --replicas=3

View pods:

kubectl get pods

Delete a pod:

kubectl delete pod <pod-name>

## Result

When one pod was deleted, Kubernetes automatically created a new pod to maintain the desired replica count.

This demonstrates Kubernetes self-healing.