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

Create a yml file and save it at /tmp/CKAQA/CKAQAq5.yml that creates a pod which has an Init container. The Init container should create a file at /opt/bonjour.txt which contains the text "Bonjour Monsieur".

Add another container to the same pod with an image of *busybox:1.28* that checks the file has the contents specified above and exits if it doesn't match "Bonjour Monsieur".

(Hint: You may have to create a volume to store this file?)
(Hint2: You can use "if grep -q 'Bonjour Monsieur' /opt/bonjour.txt; then echo 'Found it'; sleep 180; else exit 44; fi" to check the file)

---

## Question 6

Create a deployment called nginx4 in the namespace *ckaexam2* based on nginx:latest with 4 replicas and labels tier=web & app=nginx.

Create a file at /tmp/CKAQA/CKAQAq6.txt that has a list of the pods of this deployment sorted by Pod IP and has the following custom columns

* Pod Name
* Pod Status
* Pod Creation Time
* Labels

---

## Question 7

Create a Daemon Set
Check running on all nodes

---

## Question 8

Create a configmap which is exported into the a pod as an environment variable TEAM=arsenal.

The pod should run alstard/teamdemo image and you should expose the pod as a service such that you can load a webpage in your browser
on http://localhost:8888 and check the correct image is displayed.

---

## Question 9

Create a secret.... Decrypt a file which says "shhhh... this is a secret. Don't tell anyone!"

---

## Question 10

Drain a node - ensure all Daemonsets are drained too

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

Use etcdctl to backup your ETCD Cluster (provided endpoints, ca, cert, key)

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
