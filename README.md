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

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/9e3a42060580da33304ac284d9a9b54fbea5823d/img/1.png" alt="Header">
</p>
<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/9e3a42060580da33304ac284d9a9b54fbea5823d/img/2.png" alt="Header">
</p>

Для ручной установки Minikube в Windows, загрузите minikube-windows-amd64 , переименуйте его в minikube.exe И добавьте его в директорию исполняемых файлов.

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/3.png" alt="Header">
</p>
<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/4.png" alt="Header">
</p>
<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/5.png" alt="Header">
</p>

Чтобы программка видела наши команды, в среду добавляем наш путь к папке кибернетесу

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/6.png" alt="Header">
</p>
<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/7.png" alt="Header">
</p>
<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/8.png" alt="Header">
</p>

Теперь открываю VirtualBox и запускаю миникуб

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/9.png" alt="Header">
</p>

Конфигурационный файл кубера

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/10.png" alt="Header">
</p>
<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/11.png" alt="Header">
</p>

Проверка статуса, что всё нормально работает

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/12.png" alt="Header">
</p>

Можно задать определённые параметры машины

<p align="center">
  <img src="https://github.com/exeleron07/minikube-windows/blob/5bfafa9ade7208b668c6afbb4ddffeb21abd1695/img/13.png" alt="Header">
</p>

Можно подключиться через SSH

