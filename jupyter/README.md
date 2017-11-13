## Jupyter chart
#### how to deploy:
helm install jupyter --name=jupyter-yuanbowen1 --namespace=bigdata --set user=yuanbowen1 --set port=10051 --set ingress.host=jupyter-yuanbowen1.test-cloud.bigdata.wanda.cn
