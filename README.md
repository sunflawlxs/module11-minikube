# Tutorial 11 (Minikube)
Nama: Sheryl Ivana Widjaja<br>
NPM: 2206824943<br>
Kelas: Pemrograman Lanjut - A<br>

---
## REFLEKSI 1
###### 1.1. Compare the application logs before and after you exposed it as a Service. Try to open the app several times while the proxy into the Service is running. What do you see in the logs? Does the number of logs increase each time you open the app?
![](images/1.png) 
Yes, there is a difference because after the service is exposed. The service can receive requests so that the log will record requests that have been made, for example as follows if refreshed many times against the hello-node service

###### 1.2. Notice that there are two versions of `kubectl get` invocation during this tutorial section. The first does not have any option, while the latter has `-n` option with value set to `kube-system`. What is the purpose of the `-n` option and why did the output not list the pods/services that you explicitly created?
The -n option indicates that the service we want is from the namespace, which is how the two syntaxes differ from one another. This is necessary, for instance, if numerous services with the same name are dispersed among numerous namespaces. By utilizing -n, we direct the get to the namespace we provide following the -n query.  
<br>