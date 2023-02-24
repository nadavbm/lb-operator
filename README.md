# lb-operator

this repository will work with several apis and controllers

to initialise with kubebuilder with multiple groups:
```
kubebuilder init --domain example.com --repo example.com/lb
kubebuilder edit --multigroup=true
```

create the relevant api for running a load balancer instance in kubernetes:
```
kubebuilder create api --group services --version v1alpha1 --kind Service
kubebuilder create api --group configmaps --version v1alpha1 --kind ConfigMap
kubebuilder create api --group deployments --version v1alpha1 --kind Deployment
```


