# k8s-prod
Files, notes, reminders howto run stuff in my k8s env

# Hints
## Get bash inside pod
```kubectl exec -it -n nodered $(kubectl get pods --selector=app=nodered -n nodered --output=jsonpath={.items..metadata.name}) -- bash``` 

```kubectl exec -it nodered-5cb4cdf77c-klqln -n nodered -- bash```
## Enable module
Running bash inside pod ```npm install <name of module>``` 
### my modules
* node-red-contrib-telegrambot
