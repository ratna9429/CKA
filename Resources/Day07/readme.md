## Check out the task.md file for day07 task details

## Different ways of creating a Kubernetes object

- Imperative way ( Through command or API calls)
- Declarative way ( By creating manifest files)

![image](https://github.com/piyushsachdeva/CKA-2024/assets/40286378/b038c4d3-87b7-474d-a3aa-5983d978f885)

## Below is the sample pod YAML used in the video:

```YAML
# This is a sample pod yaml

apiVersion: v1
kind: Pod
metadata:
  name: nginx-pod
  labels:
    env: demo
    type: frontend
spec:
  containers:
  - name: nginx-container
    image: nginx
    ports:
    - containerPort: 80
```

# Remark: Below My Notes

1 - Create a pod using the imperative command and use nginx as the image - Done.
Command :
kubectl run nginx-pod --image=nginx:latest

2 - Now creating using declarative way. In this i have to write yaml file.
yaml file :
