Files needed to get Motioneye running in k8s.
Using nfs as persistent storage, ingress with letsencrypt certificates provided by cert manager.

# Steps
* Edit the files to change storage, ingress and so on 
* ``` kubectl apply -f motioneye ```
* Point your webbrowser to the url in the ingress yaml file.

# Extra
* The workers needs nfs tools (on Ubuntu nfs-common)
