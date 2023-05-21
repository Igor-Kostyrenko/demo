# Proof of Concept (PoC) по розгортанню GitOps системи ArgoCD на Kubernetes кластері, створеному в k3d

### Задача

Розгорнути Kubernetes кластер за допомогою **k3d** та встановити ArgoCD

#### Інсталяція

1.1 Створюємо Kubernetes кластер, за допомогою наступної команди:

> k3d cluster create argo -s 1 -a 3

1.2 Розгортаємо AgroCD в namespace 'argocd':

> kubectl create namespace argocd
> kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

1.3 Після закінчення розгортання надаємо доступ до графічного інтерфейсу ArgoCD за допомогою Port Forwarding:

> kubectl port-forward service/argocd-server -n argocd --address 0.0.0.0 8080:443 > /dev/null&

1.4 Отримаємо тимчасовий пароль адміністратора для першого входу в систему:

> kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo

#### Конфігурація

2.1 Для доступу до графічного інтерфейсу необхідно в браузері набрати:


> 127.0.0.1:8080
