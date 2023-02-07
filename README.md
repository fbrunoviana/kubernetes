# Kubernetes

---
## O que é Kubernetes
- O Kubernetes é um sistema de gerenciamento de contêiner.
- É open-source e foi criado por Google.
- Oferece uma plataforma para implantação, escalabilidade e gerenciamento de aplicações em contêineres.
- Fornece uma estrutura de automação para garantir a disponibilidade e escalabilidade de aplicativos.
- Possibilita a implantação e atualização de aplicativos sem interrupção.
- Permite a gestão de recursos para aplicativos, como CPU, memória e armazenamento.
- Oferece escalabilidade automática de recursos de acordo com a demanda.
- Possibilita a execução de testes de integração e entrega contínua.
- Oferece uma camada de segurança para aplicações.
### Chave:
O Kubernetes é uma plataforma de gerenciamento de contêiner open-source que oferece automação para implantação, escalabilidade, gerenciamento de recursos e segurança de aplicações em contêineres.

---

 Veja mais em: [Documentação](https://kubernetes.io/pt-br/docs/concepts/overview/what-is-kubernetes/)

---


## Componentes do Kubernetes
- Nó (Node): Um nó é um servidor que executa aplicativos em contêineres.
- Cluster: Um cluster é uma coleção de nós que trabalham juntos para executar aplicações.
- Control Plane: O control plane é responsável por gerenciar o estado desejado do cluster.
- API Server: O API Server é o ponto de entrada para o control plane, que recebe solicitações de gerenciamento e atualizações de estado.
- etcd: O etcd é um banco de dados de chave-valor distribuído que armazena o estado configurado do cluster.
- Controller Manager: O Controller Manager é responsável por gerenciar controladores, como o Replication Controller.
- Scheduler: O Scheduler é responsável por alocar nós para aplicativos.
- Kubelet: O Kubelet é responsável por garantir que os contêineres estejam executando em um nó.
- Kube-Proxy: O Kube-Proxy é responsável por gerenciar o acesso à rede para aplicativos.
### Chave:
Os componentes do Kubernetes incluem nós, cluster, control plane, API Server, etcd, Controller Manager, Scheduler, Kubelet e Kube-Proxy, cada um com uma função específica na gestão e execução de aplicativos em contêineres.

---

Veja mais em: [Documentação](https://kubernetes.io/pt-br/docs/concepts/overview/components/)

---


## Objetos do Kubernetes
- Pod: Um Pod é o menor e mais básico objeto de implantação em um cluster do Kubernetes, contendo um ou mais contêineres.
- Service: Um Service é usado para expor um conjunto de Pods como uma única entidade lógica para outros componentes do cluster.
- Volume: Um Volume é um recurso de armazenamento compartilhado entre os contêineres em um Pod.
- Namespace: Um Namespace é usado para separar recursos do cluster em ambientes lógicos.
- ConfigMap: Um ConfigMap é usado para armazenar dados de configuração não sensíveis.
- Secret: Um Secret é usado para armazenar dados sensíveis, como credenciais.
- Deployment: Um Deployment é usado para gerenciar a implantação de uma nova versão de um aplicativo.
- StatefulSet: Um StatefulSet é usado para gerenciar a implantação de aplicativos que precisam preservar estado entre reinicializações.
- Job: Um Job é usado para executar tarefas únicas e garantir que sejam concluídas com sucesso.
### Chave:
Os objetos do Kubernetes incluem Pods, Services, Volumes, Namespaces, ConfigMaps, Secrets, Deployments, StatefulSets e Jobs, cada um com uma função específica na implantação e gestão de aplicativos em um cluster do Kubernetes.

---
Veja mais em: [Documentação](https://kubernetes.io/pt-br/docs/concepts/overview/working-with-objects/kubernetes-objects/)

---


## Relatório de Análise da Gestão de Objetos do Kubernetes
- kubectl: O kubectl é a ferramenta de linha de comando usada para gerenciar objetos do Kubernetes.
- Manipulação de objetos: A manipulação de objetos inclui criar, atualizar, listar e excluir objetos do cluster.
- Labels e annotations: Labels e annotations são usados para identificar e adicionar informações adicionais aos objetos do cluster.
- Garbage Collection: O Garbage Collection é usado para excluir automaticamente objetos não mais necessários.
- Liveness e Readiness Probes: As probes de liveness e readiness são usadas para verificar se um aplicativo está executando corretamente.
### Chave:
A gestão de objetos do Kubernetes inclui a ferramenta kubectl, a manipulação de objetos, labels e annotations, o Garbage Collection e as probes de liveness e readiness, todas usadas para garantir a correta implantação e operação de aplicativos em um cluster do Kubernetes.

---

Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/object-management/)

---


## Nomes de Objetos do Kubernetes
- Nomes qualificados: Os nomes qualificados são nomes completos de objetos no cluster, incluindo o namespace e o nome do objeto.
- Nomes curtos: Os nomes curtos são nomes simples de objetos no cluster, sem incluir o namespace.
- Nomes únicos: Todos os nomes de objetos no cluster devem ser únicos dentro de um namespace.
- Alocação de nomes: A alocação de nomes é o processo de atribuição de um nome a um novo objeto.
### Chave:
Os nomes de objetos no Kubernetes são qualificados, curtos e únicos dentro de um namespace, e a alocação de nomes é o processo de atribuir um nome a um novo objeto.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/)



---


## Rótulos de Objetos do Kubernetes
- Função: Rótulos são usados para identificar e classificar objetos no cluster.
- Formato: Rótulos são compostos por uma chave e um valor.
- Atribuição: Rótulos são atribuídos a objetos durante sua criação ou atualização.
- Uso: Rótulos são usados para selecionar conjuntos de objetos com base em suas características.
### Chave:
Os rótulos são usados para identificar e classificar objetos no cluster do Kubernetes, e são compostos por uma chave e um valor. São atribuídos durante a criação ou atualização de objetos e são usados para selecionar conjuntos de objetos com base nas suas características.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/)

---


## Namespaces em Kubernetes
- Função: Namespaces são usados para agrupar objetos em um cluster do Kubernetes.
- Criação: Namespaces são criados para agrupar objetos relacionados e para facilitar a gestão de recursos.
- Uso: Namespaces são usados para isolar objetos e recursos em um cluster do Kubernetes.
- Limitações: Cada namespace tem suas próprias limitações de recursos, como CPU, memória e armazenamento.
### Chave:
Os namespaces são usados para agrupar objetos relacionados e para isolar recursos em um cluster do Kubernetes. Eles são criados para facilitar a gestão de recursos e têm suas próprias limitações de recursos.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/)

---


## Anotações em Kubernetes
- Função: As anotações são usadas para adicionar metadados a objetos no cluster do Kubernetes.
- Formato: As anotações são compostas por uma chave e um valor.
- Atribuição: As anotações são atribuídas a objetos durante sua criação ou atualização.
- Uso: As anotações são usadas para armazenar informações adicionais sobre objetos no cluster, como informações de versionamento ou informações de gerenciamento de configurações.
### Chave:
As anotações são usadas para adicionar metadados a objetos no cluster do Kubernetes. São compostas por uma chave e um valor, atribuídas durante a criação ou atualização de objetos, e usadas para armazenar informações adicionais sobre objetos no cluster.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations/)


---


## Seletores de Campos em Kubernetes
- Função: Seletores de campos são usados para filtrar objetos no cluster do Kubernetes.
- Formato: Seletores de campos são expressões que correspondem a campos específicos em objetos no cluster.
- Uso: Seletores de campos são usados para filtrar objetos para ações, como listagens, exibições, atualizações e exclusões.
- Exemplos: Alguns exemplos de seletores de campos incluem selecionar objetos com um determinado nome ou com uma determinada etiqueta.
### Chave:
Seletores de campos são usados para filtrar objetos no cluster do Kubernetes. São expressões que correspondem a campos específicos em objetos e são usados para filtrar objetos para ações, como listagens, exibições, atualizações e exclusões.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/field-selectors/)


---


## Finalizadores em Kubernetes
- Função: Os finalizadores são usados para garantir ações de limpeza em objetos no cluster do Kubernetes.
- Adição: Finalizadores podem ser adicionados a objetos durante sua criação ou atualização.
- Funcionamento: Quando um objeto é marcado para exclusão, o Kubernetes executa qualquer ação especificada pelo finalizador antes de excluir o objeto.
- Uso: Finalizadores são usados para garantir ações de limpeza antes da exclusão de objetos, como desalocar recursos ou excluir dependências.
### Chave:
Finalizadores são usados para garantir ações de limpeza em objetos no cluster do Kubernetes. Podem ser adicionados a objetos durante sua criação ou atualização, são executados pelo Kubernetes antes da exclusão de objetos, e são usados para garantir ações de limpeza antes da exclusão, como desalocar recursos ou excluir dependências.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/finalizers/)

---


## Proprietários e Dependentes em Kubernetes
- Função: Proprietários e dependentes são conceitos utilizados para gerenciar a vida útil de objetos no cluster do Kubernetes.
- Proprietários: Objetos podem ser definidos como proprietários de outros objetos. Isso significa que o objeto proprietário tem um relacionamento de dependência com os objetos dependentes.
- Dependentes: Objetos dependentes são aqueles que têm um relacionamento de dependência com um objeto proprietário.
- Uso: Proprietários e dependentes são usados para garantir que objetos dependentes sejam criados, atualizados ou excluídos junto com seus objetos proprietários.
### Chave:
Proprietários e dependentes são conceitos utilizados para gerenciar a vida útil de objetos no cluster do Kubernetes. Objetos podem ser definidos como proprietários de outros objetos, e os objetos dependentes têm um relacionamento de dependência com os objetos proprietários. Esses conceitos são usados para garantir que objetos dependentes sejam criados, atualizados ou excluídos junto com seus objetos proprietários.

---
Veja mais em: [Documentação](https://kubernetes.io/docs/concepts/overview/working-with-objects/owners-dependents/)

---
