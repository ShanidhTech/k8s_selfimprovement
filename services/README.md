## ClusterIP


![image](https://github.com/user-attachments/assets/556c52c9-b923-4ae3-815a-b59ec3930a39)


Its primary purpose is to expose a Service on a cluster-internal IP address. This means the Service is only reachable from within the Kubernetes cluster.


## Nodeport


![image](https://github.com/user-attachments/assets/892d04ad-83ef-4b06-804c-5fbb79b06360)


The NodePort Service exposes the Service on a static port on each Node in the cluster. This allows external traffic to reach your application by connecting to any Node's IP address on the specified NodePort.
