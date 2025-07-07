## ClusterIP


![image](https://github.com/user-attachments/assets/556c52c9-b923-4ae3-815a-b59ec3930a39)


Its primary purpose is to expose a Service on a cluster-internal IP address. This means the Service is only reachable from within the Kubernetes cluster.


![image](https://github.com/user-attachments/assets/44dc19b3-b4d5-4320-bc85-f40a25a997c2)
#### 1. Create a test pod to access the service 

`kubectl run test-client --rm -it --image=busybox --restart=Never -- sh`

#### 2. Test the service inside the shell

`wget -qO- http://backend-service`


## Nodeport


![image](https://github.com/user-attachments/assets/892d04ad-83ef-4b06-804c-5fbb79b06360)

The NodePort Service exposes the Service on a static port on each Node in the cluster. This allows external traffic to reach your application by connecting to any Node's IP address on the specified NodePort.


![image](https://github.com/user-attachments/assets/c903a6e2-2700-4e00-b9eb-a6972467f19a)

try running `kubectl get nodes -o wide` to see the IP of the "node" (which might be 127.0.0.1 or an internal Docker network IP) and test that.

![image](https://github.com/user-attachments/assets/665ee8b7-0842-4b58-9271-18ebbaac7489)
