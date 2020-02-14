# Exam style questions for the CNCF CKA Exam

## Question 1

List all the PV's in the cluster and sort them by name (use kubectl sorting only)

---

## Question 2

Deploy a pod called *tdq2* using the alstard/teamdemo image in namespace q2.

Output the logs for the pod and save them in a file called /tmp/CKAQA/CKAQAq2.txt 

---

## Question 3

List all the nodes available in your cluster that do not have the label *unreachable*, sort them by Internal IP and write the output of the listing to a file at /tmp/CKAQA/CKAQAq3.txt

---

## Question 4

Create a pod named *web* using the nginx:1.16.1 and schedule this pod on a node labelled with *disk = ssd*

---

## Question 5

Create a yml file and save it at /tmp/CKAQA/CKAQAq5.txt that creates a pod which has an Init Container. The init container should create a file at /opt/bonjour.txt which contains the text "Bonjour Monsieur" - use any image you like for this (Hint: use *busybox:1.28*)

Add another container based on *busybox:1.28* that checks this file exists and has the contents specified above and exits if it does not

---

## Question 6

Specify the pod to create a name in the namespace test, containing four specified mirror nginx, redis, memcached, busybox

---

## Question 7

Create a pod name Test, the mirror is Nginx, Volume name cache-volume is hanging in / data directory, and Volume is the non-Persistent

---

## Question 8

List pod in the Service named test and find out using one of the highest CPU utilization, the pod written to the file name

---

## Question 9

Create a Pod name for nginx-app, mirroring as nginx, and nginx-app create a Service named according pod, type is NodePort

---

## Question 10

Create a nginx's Workload, to ensure that run on each node, careful not to overwrite the original node Tolerations

---

## Question 11

The deployment of the number of copies from 1 nginx-app becomes 4.

---

## Question 12

Create deployment nginx-app using a mirror image nginx: 1.11.0-alpine, to modify the image 1.11.3-alpine, and record update, then rollback, mirroring rollback to nginx: 1.11.0-alpine

---

## Question 13

The pod has a nginx to create svc named nginx, and use nslookup to find out the service dns records, pod and the dns records are written to the specified file

---

## Question 14

Create named MySecret Secret, the password field contains a value of Bob, then call in the ENV pod1 Lane, Volume POD2 in use mounted at / data

---

## Question 15

Node1 node 15. Although not scheduled, and redistributed on the pod node

---

## Question 16

Use etcdctl to backup your ETCD Cluster (provided enpoints, ca, cert, key)

---

## Question 17

give a loss associated cluster node, node failure investigation, to ensure that the change is permanent.

---

## Question 18

Create a pv, type hostPath, located in / data, the size of 1G, mode ReadOnlyMany

---

## Question 19

Given cluster, add the node to the cluster node1, using TLS bootstrapping

---
