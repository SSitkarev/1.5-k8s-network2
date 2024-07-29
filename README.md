# Домашнее задание к занятию «Сетевое взаимодействие в K8S. Часть 2» - Сергей Ситкарёв

## Задание 1. Создать Deployment приложений backend и frontend

Создать Deployment приложения frontend из образа nginx с количеством реплик 3 шт.

[front](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/src/front.yaml)

Создать Deployment приложения backend из образа multitool.

[back](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/src/back.yaml)

Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера.

[service](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/src/service.yaml)

Продемонстрировать, что приложения видят друг друга с помощью Service. Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

![Задание1](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/img/1.jpg)

## Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера

Включить Ingress-controller в MicroK8S.

![Задание2](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/img/2.jpg)

Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался frontend а при добавлении /api - backend.

[ingress](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/src/ingress.yaml)

Продемонстрировать доступ с помощью браузера или curl с локального компьютера. Предоставить манифесты и скриншоты или вывод команды п.2.

![Задание2](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/img/3.jpg)

![Задание2](https://github.com/SSitkarev/1.5-k8s-network2/blob/main/img/4.jpg)