# helm-starter
Starter template for helm charts. 

## Why
Standard helm scaffolding is too limited (i.e. doesn't have any predefined settings for env), and at the same time make certain assumptions about your service which has to be addressed before deploying (liveness and readiness probes). 
That's why I created this starter template which improves (imho) things a little bit. 

## Usage
when creating a new helm template, pass `-p` parameter with **absolute** path to your starter template, i.e.
```
helm create -p $(pwd)/starter mychart
```
