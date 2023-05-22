# Розгортання додатку та автоматична синхронізація в ArgoCD  

### Інсталяція

1.1 Створюємо Kubernetes кластер, за допомогою наступної команди:

> k3d cluster create argo

1.2 Розгортаємо AgroCD в namespace 'argocd':

> kubectl create namespace argocd
> kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

1.3 Після закінчення розгортання надаємо доступ до графічного інтерфейсу ArgoCD за допомогою Port Forwarding:

> kubectl port-forward service/argocd-server -n argocd --address 0.0.0.0 8080:443

1.4 Отримаємо тимчасовий пароль адміністратора для першого входу в систему:

> kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo

1.5 Змінемо тимчасовий пароль адміністратора на власний в графічному інтерфейсі у вкладці ***User info***

#### Конфігурація

2.1 Створення додатку за допомогою графічного інтерфейсу argocd:



