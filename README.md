# Kubernetes на Windows

В этом проекте демонстрируется работа поднятия кластера kubernetes. Нам потребуется установить три приложения: 1) VirtualBox - https://www.virtualbox.org/  2) Kubectl - https://kubernetes.io/docs/tasks/tools/install-kubectl/   3) Minicube - https://kubernetes.io/docs/tasks/tools/install-minikube/    VirtualBox - нужен для создания виртуального сервера на вашем компьютере, где будет создан K8s Cluster. Kubectl - для управления K8s кластером.
---

## Основные команды Kubernetes

- `minikube version` — Показать версию minicube
- `minikube start` — Создать и Запустить VM с K8s Cluster с параметрами по умолчанию
- `minikube stop` - Остановить VM с нашим K8s Cluster
- `minikube delete` - Удалить VM с нашим K8s Cluster
- `minikube ssh` - Сделать Login на VM с нашим K8s cluster

- `minikube start --cpus=4--memory=8gb --disk-size=5gb` - Создать и Запустить VM с K8s Cluster с нашими параметрами
- `minikube start --cpus=2--memory=6000mb --disk-size=4000mb` - Создать и Запустить VM с K8s Cluster с нашими параметрами
- `minikube start -p MYSUPERCLUSTER`- Создать и Запустить VM с K8s Cluster с нашим именем

- `kubectl version` - Показать версию kubectl client'a и сервера
- `kubectl version --client` - Показать версию kubectl client'a
- `kubectl get componentstatuses` - Показать состояние K8s Cluster'a
- `kubectl cluster-info` - Показать информацию о K8s Cluster'e
- `kubectl get nodes` - Показать все Серверы K8s Cluster'a

---
