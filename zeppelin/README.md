## Zeppelin chart
#### how to deploy:
helm install zeppelin --name=zeppelin-yuanbowen1 --namespace=bigdata --set user=yuanbowen1 --set allowed_users=yuanbowen1 --set port=8091 --set ingress.host=zeppelin-yuanbowen1.test-cloud.bigdata.wanda.cn
