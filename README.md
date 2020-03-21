# kubebuilder-demo

Basic getting started of kubebuilder SDK.

1. To generate code,

```bash
$ make
```

2. To install the CRD,

```bash
$ make install
```

3. To run controller in Local,

```bash
$ make run
```

Without webhooks,

```console
$ make run ENABLE_WEBHOOKS=false
```

Deploy Controller in cluster,

```bash
$ make docker-build docker-push IMG=<some-registry>/<project-name>:tag
$ make deploy IMG=<some-registry>/<project-name>:tag
```

4. To install sample Crontab custom resource,

```bash
$ kubectl apply -f config/samples/
```