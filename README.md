# kube-command
Комманды при изучений kubernetes

## Minikube
Запустить миникуб машин и запустить кластеры которые ранее запускались:
```
minikube start
```
Удалить кластер:
```
minikube delete
```

Изменить виртуалку в minikube:
```
minikube config set driver docker
```

## Kubectl

Запустить pod с манифест файлом:
```
kubectl create -f ./pod.yaml
```

Список запущенных pods
```
kubectl get pod
```

Удалить под названию (вместо --all) или все
```
kubectl delete pod --all
```

Запустить pod с манифест файлом:
```
kubectl create -f ./replicaset.yaml
```

Список запущенных replicaset 
```
kubectl get replicaset
```

## Советы
Если
```
$ kubectl get pod
my-pod   0/1     ImagePullBackOff   0          16m
```
нужно установить нужный docker image который ты указал в yaml файле

## Полезные ссылки:
#### Ссылки:
- [minikube](https://minikube.sigs.k8s.io/)
- [kubernetes](https://kubernetes.io/ru/docs/setup/learning-environment/minikube/#%D1%83%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B4%D1%80%D0%B0%D0%B9%D0%B2%D0%B5%D1%80%D0%B0-%D0%B2%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D0%BE%D0%B9-%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%D1%8B)
#### Доклады:
- [Кластер Kubernetes в твоём ноутбуке. Знакомство с minikube / Виктор Сафронов (Авито)](https://www.youtube.com/watch?v=7I_FreB0Cu0&t=1831s&ab_channel=HighLoadChannel)
#### Вебинары:
- [Вечерняя школа Слёрма по Kubernetes.](https://www.youtube.com/watch?v=Jp866ltZBSk&list=PL8D2P0ruohOA4Y9LQoTttfSgsRwUGWpu6&ab_channel=%D0%A1%D0%BB%D1%91%D1%80%D0%BC)
