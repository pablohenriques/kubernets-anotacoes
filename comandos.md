- visualizar pods:
    kubectl get pods

- visualizar construção pods:
    kubectl get pods --watch

- visualizar detalhes de um pod:
    kubectl describe pod <nome-do-pod>

- deletar um pod
    kubectl delete -f <nome-do-arquivo-configuração> ou <path/arquivo-configuracao>
    kubectl delete pod <nome-do-pod>

- acessar pod via terminal:
    kubectl exec -it <nome-do-pod> -- bash (`sim, menos menos espaco bash`)
    - ctrl + d: sai do terminal

- apresentar pods com ip:
    kubectl get pods -o wide

- apresentar IPs para o mundo externo
    minikube start --vm-driver=virtualbox

- deletar todos os pods:
    kubectl delete pods --all