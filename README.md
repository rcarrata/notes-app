# notes-app
Notes App deployed in Openshift 4 for Mesh testing purposes

## Deployment in OCP4

```
oc adm policy add-scc-to-user anyuid -z default
oc new-app https://github.com/rcarrata/notes-app.git --name=notes-app
oc expose svc/notes-app
```

## TODO

- Run as non root
- Change to ubi8/python-36
