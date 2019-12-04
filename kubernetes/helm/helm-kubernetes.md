# Airflow installation on Kuberenetes using Helm Charts.

```
helm install stable/airflow
```

```
helm install stable/airflow --namespae airflow --name airflow -f values.yaml
```