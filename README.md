# Arquivos de configuração de um cluster kubernetes novo
Esse repositorio irá gerar um release contendo os arquivos .yaml que precisarão ser aplicados em um cluster kubernetes recém provisionado.
Então inclusos:
- Cert manager: é baixada a versão latest do cert manager
- Ingress controler: é gerado e parametrizado o arquivo de provisionamento do ingress controler nginx para nuvem OKE ~~e também para AWS~~
- Cluster issuer: é gerado um arquivo padrão de Issuer de certificados Letsencrypt
- Dashboard: é gerado um arquivo parametrizado para o provisionamento da dashboard K8S
- Deployment Exemplo: é gerado um arquivo parametrizado de um webserver exemplo nginx com ingress e ssl
~~- Metrics server: é baixada a versão latest do metrics server, necessário para proivisionamento do cluster autoscaler~~
~~-Cluster autoscaler: é baixado e parametrizado o arquivo de provisionamento do cluster autoscaler OKE e AWS~~

# Como Usar
1- Navegue para as Actions:
![image](https://user-images.githubusercontent.com/83661016/181553999-cc910a37-cfab-477b-9a0e-19a8138cd7d6.png)
2- Selecione Manual Workflow
3- Clique em Run Workflow
![image](https://user-images.githubusercontent.com/83661016/181557673-1f3fa468-783e-465f-a827-1cfcc052a2b0.png)
4- Parametrize o workflow de acordo com sua necessidade
![image](https://user-images.githubusercontent.com/83661016/181558676-370c9dde-3642-48e0-9310-4d29508f797d.png)
5- Aguarde a execução do workflow, voce pode acompanhar a execução clicando nele
![image](https://user-images.githubusercontent.com/83661016/181560026-9c9b5b93-8404-4a9b-af1b-fe33d97e5ae3.png)
![image](https://user-images.githubusercontent.com/83661016/181560367-d82588b3-8e67-4f68-ac93-1125d2a22a92.png)
6- O link do release ficará disponivel no passo "Link do Release", clique no link
![image](https://user-images.githubusercontent.com/83661016/181561308-8551fc43-2fdc-4aea-8973-e0750c5dadff.png)
7- Os arquivos gerados estarão no .zip disponivel para download
![image](https://user-images.githubusercontent.com/83661016/181562771-b2c536ed-0f66-498f-982c-555138343992.png)
8- O .zip contém os arquivos nomeados na ordem que devem ser aplicados no cluster
![image](https://user-images.githubusercontent.com/83661016/181563876-c3e30aa3-4bf9-4c01-a8c9-49f9d1940366.png)
