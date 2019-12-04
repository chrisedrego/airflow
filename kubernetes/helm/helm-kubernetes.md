# Airflow installation on Kuberenetes using Helm Charts.

- Airflow is infact made of multiple components which work together in accordance.

- Quick overview Airflow is made of the following components mentioned below:
    - Server
    - Scheduler
    - Web Server
    - Database.

- Quick an easy way to setup Airflow on Kubernetes is using the Helm chart.


```
helm install stable/airflow
```

```
helm install stable/airflow --namespae airflow --name airflow -f values.yaml
```


