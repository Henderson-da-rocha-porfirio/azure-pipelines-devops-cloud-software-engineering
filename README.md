# azure-pipelines-devops-cloud-software-engineering

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’07” (1)](https://user-images.githubusercontent.com/46926951/230672638-55823f08-0bdc-4c2d-91a9-9e97de4e0649.jpg)



---

- 1 - [Cultura DevOps](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#muito-mais-que-ferramenta-%C3%A9-cultura)
- 2 - [DevOps](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#devops)
- 3 - [ CI - Continuos Integration - Integração Contínua](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#ci---integra%C3%A7%C3%A3o-cont%C3%ADnua)
- 4 - [ CD - Continuos Deploy - Implantação Contínua](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#cd---deploy-cont%C3%ADnuo)
- 5 - [ CD- Continuos Delivery - Entrega Contínua](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#princ%C3%ADpios-da-entrega-cont%C3%ADnua--cd--continuos-delivery---)
- 6 - [ Azure DevOps - Serviços e Recursos](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#azure-devops--servi%C3%A7os-e-recursos-)
- 7 - [ Azure Pipeline ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#azure-pipelines---%C3%A9-o-tema-deste-reposit%C3%B3rio--realiza%C3%A7%C3%A3o-da-entrega-cont%C3%ADnua-)
- 8 - [ YAML ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#yaml----acr%C3%B4nimo-para-yaml-aint-markup-language)
- 9 - [ TDD ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#tdd---test-driven-development--desenvolvimento-orietado-a-teste-)
- 10 - [ Cloud - Scaling - Escalonamento ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#cloud---escalonamento)
- 11 - [ Deployment Patterns - Estratégias de implantação (deployment) ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#deployment-patterns---estrat%C3%A9gia-de-implanta%C3%A7%C3%A3o)
- 12 - [ Kubernetes - k8s ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#kubernetes---k8s)
- 13 - [ Infraestrutura em Código (IaC) ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#infraestrutura-em-c%C3%B3digo-iac)
- 14 - [ Devops Databases ](https://github.com/Henderson-da-rocha-porfirio/azure-pipelines-devops-cloud-software-engineering#devops-databases)

- 15 - [Usando o Flyway]()
---

### Muito mais que ferramenta, é cultura!

- A `antiga` cultura é baseado no modelo `humano` para provisionar ambientes. E este movimento de infraestrutura como código (IaC) veio para mudar porque traz consigo a cultura `nova` onde tudo é versionado e automatizado eliminando clicks e mais clicks.

- Provisionar recursos utilizando `scripts` é possível trazer a `infraestrutura` cada vez mais próxima do `desenvolvimento`. E também o desenvolvimento mais próximo da infraestrutura. E isso torna a cultura `DevOps` mais forte nos times da empresa.

- E o maior desafio é mudar a `cultura` e diminuir a curva de aprendizagem.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’33”](https://user-images.githubusercontent.com/46926951/229618786-7544479a-00f1-455a-ade2-7b0e12805655.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’19”](https://user-images.githubusercontent.com/46926951/229618413-86fe0d4a-4820-4950-880d-9d6a556931d8.jpg)

---

![image](https://user-images.githubusercontent.com/46926951/229619606-41e98f0d-1777-441a-897c-af4323809031.png)


---

### Dev => Mudança contínua

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’51”](https://user-images.githubusercontent.com/46926951/229619974-a22ffce2-6be8-40bc-8376-da1ae3fef20f.jpg)

---

## Ops => Estabilidade Contínua

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’04”](https://user-images.githubusercontent.com/46926951/229620459-84d061bb-15d7-497b-9e10-ad6d092b10a5.jpg)

---

## DevOps

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’12”](https://user-images.githubusercontent.com/46926951/229620704-b217c9eb-849e-4018-b6bf-5be0a656da7e.jpg)

---

## Exemplo prático do funcionamento DevOps entre equipes

### Equipe de Devs (dev) lança um novo produto:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’22”](https://user-images.githubusercontent.com/46926951/229621103-39aa46ff-9e33-4460-a9d3-0b8c68327795.jpg)

---

###  E a equipe de operação(ops) precisa manter o software no ar sem falhas

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’27”](https://user-images.githubusercontent.com/46926951/229621446-d6d5ecba-3ac7-4c95-9e50-71b785eb5f9f.jpg)

---

# Azure contribuindo no CI (integração contínua) e no CD (deploy contínuo)

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’19”](https://user-images.githubusercontent.com/46926951/229618573-6321a4eb-8ee8-411e-b926-31cbf43e6813.jpg)

---

## CI - Integração Contínua

---
### `Artefatos`: - Ajuda no planejamento ( camada de negócio com planejamento, backlog, board, métrica e etc )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’54”](https://user-images.githubusercontent.com/46926951/229622762-790be4cb-47b5-4469-9708-d565586b0297.jpg)

---

### `Repositórios`: Ajuda no desenvolvimento ( camada de desenvolvimento de código com um tipo de versionador similar ao git e etc ). A Microsoft disponibiliza Ide's como nas da imagem que se integram ao Azure.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’31”](https://user-images.githubusercontent.com/46926951/229627548-bf030e28-45d7-4024-ab98-545b974020f2.jpg)

---

### `Ambiente de Testes Unitários`: Começo da integração com o Build ( camada de testes unitários )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’48”](https://user-images.githubusercontent.com/46926951/229623499-7a530a0f-1b23-4051-a53a-0cc5b3c2f39b.jpg)


---

### `Ambiente de Homologação`: Realizando testes da aplicação já em homologação ( camada de testes da aplicação simulando a prod mas em nível de desenvolvimento, geralmente onde os testers trabalham ). Esta fase é o limite entre o Dev e o Ops


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’30”](https://user-images.githubusercontent.com/46926951/229624476-a2a05cd5-f291-4f27-a720-0a109f6d75c8.jpg)

---

#### Selênio pode ser utilizado, caso deseje, para ajudar também nesta camada de testes de automação

![image](https://user-images.githubusercontent.com/46926951/229628145-4a65e5ce-1d9f-4eab-a135-1940b6313c3b.png)


---

## CD - Deploy Contínuo

---

### `Ambiente de Staging`: Implantação (release)- garante a entrega com velocidade e de maneira automática ( camada de staging - ambiente idêntico ao da produção. Algum erro aqui, também estará na produção caso não tenha sido corrigido )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’50”](https://user-images.githubusercontent.com/46926951/229625497-a812a035-5ad8-4efb-b4d9-5f96579cdcea.jpg)


---

### `Deploy`: ambiente da produção. Azure também pode fazer uso do docker. ( podendo integrar com o Docker para instanciar containers e também o kubernetes para orquestrar os mesmos )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’07”](https://user-images.githubusercontent.com/46926951/229628562-0435f663-3462-4d5e-8257-7558897be7db.jpg)


---

### `Operate`: camada de operações em nível de infraestrutura como código

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’32”](https://user-images.githubusercontent.com/46926951/229629332-788b9c30-7295-4ff5-92b9-75b23c66e369.jpg)


--- 

###  Integração com o Terraform


- Terraform is an open source tool developed and maintained by HashiCorp that has the exact same goal than ARM templates: it helps you to describe your infrastructure, using HCL (HashiCorp Configuration Language) which is more readable than JSON, and then deploy it to Azure. It comes with a set of tools that also help you to manage the state and lifecycle of your deployments, which makes it a bit more advanced than ARM templates. Also, Terraform is not only working with Microsoft Azure, but also with a ton of other providers (the full list is available here). That does not mean that when you write an HCL template for Microsoft Azure, then it can be used to deploy on any other cloud magically. No, that means that you will be able to use the same language and tools to automate the way you deploy a specific infrastructure on any platforms supported by Terraform. Trust me, it’s something big!


![image](https://user-images.githubusercontent.com/46926951/229629797-972d1752-fdbc-4d8b-ba6a-6bb608cc05f6.png)

---


# Azure DevOps ( Serviços e Recursos )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’50”](https://user-images.githubusercontent.com/46926951/229632362-8ea15dff-f9f4-40b2-93d4-2066ce0d1246.jpg)


---

## Azure DevOps Services

### Azure Artifacts

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’57”](https://user-images.githubusercontent.com/46926951/229634327-b95517b3-c648-40a6-a3e7-7d4ffcf06818.jpg)


---


### Azure Boards - gerenciamento de projetos ( backlog - planejamento - cards )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’55”](https://user-images.githubusercontent.com/46926951/229633176-ed0dcbfe-1779-4c80-8ad1-83f2aa7e05d5.jpg)


---

### Azure Repos ( repositorios )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’24”](https://user-images.githubusercontent.com/46926951/229633859-7c786721-03b7-4d7b-9484-2d5989a8918e.jpg)


--- 


### Azure Test Plans

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’37”](https://user-images.githubusercontent.com/46926951/229634090-68b476c2-45a9-4bab-8f8d-bf9096a733e4.jpg)

---

### Azure Pipelines - é o tema deste repositório ( realização da entrega contínua )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’19”](https://user-images.githubusercontent.com/46926951/229633543-67e5ee10-ff7f-4819-8ed2-2f4174c88fe9.jpg)


---


## Azure Dashboard

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-21’25”](https://user-images.githubusercontent.com/46926951/229634779-d84e37bb-bfb0-48ee-87f3-5598f27a4a1a.jpg)


---

## YAML -  acrônimo para YAML Ain't Markup Language.

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’58”](https://user-images.githubusercontent.com/46926951/229640746-75cfcce4-db4b-4256-b6b7-0df1200d6dd5.jpg)

---

- Formato de serialização de dados legíveis para seres humanos.

- Ele é o substituto para o .XML

- Vantagem de alterar a configuração da Pipeline sem precisar entrar no Azure DevOps:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’29”](https://user-images.githubusercontent.com/46926951/229637181-6f01b633-1cb7-4762-8195-3c48529a0ccc.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’37”](https://user-images.githubusercontent.com/46926951/229637279-a7716b4c-9e17-48ae-bf29-7e884599e42b.jpg)


---

### Listas ficam entre colchetes `[]`:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’49”](https://user-images.githubusercontent.com/46926951/229637527-2c24a051-787c-4121-ae35-4cb5faa6c7e6.jpg)


---

### Vetores Associados

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’56”](https://user-images.githubusercontent.com/46926951/229637705-f05265cb-abee-4d87-b30e-7390dbc08c9d.jpg)

---

### Comentários

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’13”](https://user-images.githubusercontent.com/46926951/229637876-6b2e7f99-cb56-4379-8dd2-cabf269fb04a.jpg)

---

### YML na raiz do repositório - configuração de pipeline

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’54” (1)](https://user-images.githubusercontent.com/46926951/229638102-3d20da75-7667-4a3f-9224-799c737187d6.jpg)


---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’00”](https://user-images.githubusercontent.com/46926951/229638245-6d192026-a052-42f3-bd2b-a761bb817a83.jpg)


---

### Início do Pipeline

### Trigger - opcional ( esse gatilho diz ao pipeline o que ele deve começar a rodar podendo ser acionado manualmente ou automaticamente )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’10”](https://user-images.githubusercontent.com/46926951/229638405-01357997-d6ba-42ec-9e9f-ca1c0f4e121d.jpg)

---


### Stages do Pipeline ( estágios ) - usado para marcar alguns pontos importantes como a compilação, controle de qualidade e a produção

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’56” (1)](https://user-images.githubusercontent.com/46926951/229638735-37b2afed-810c-4849-8703-f0524c45e7a1.jpg)


---

### Dentro dos Stages temos os `Agents Jobs` ou simplesmente os `Agents` ( servidores que vão processar e executar as ações que precisamos na `CI`:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’11”](https://user-images.githubusercontent.com/46926951/229639115-585afea4-ca10-4e1e-8c94-bd0dab15e56e.jpg)

---

### Especificações dos Recursos que ficam dentro dos Agents para a execução do pipeline ( dependsOn ):

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’37”](https://user-images.githubusercontent.com/46926951/229639481-a2d068e4-6850-42ab-a714-61a7571063ab.jpg)

---

### Jobs - Define a sequência de execução de um conjunto de steps


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’50” (1)](https://user-images.githubusercontent.com/46926951/229639692-29bed0b1-e6f5-4411-b50b-b9bc4c4f393b.jpg)


---

### Templates - podem ser usados dentro do YAML ( evita repetição de configurações )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’08”](https://user-images.githubusercontent.com/46926951/229639871-7920713b-d68d-4f41-b711-2bd589968b8a.jpg)

---


### Tasks - ( tarefas que executam uma ação: rodar comando shell, fazer testes unitários ou publicar um artefato )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’28”](https://user-images.githubusercontent.com/46926951/229640095-9d28fddc-f5a2-49ba-8970-a9352a53ba91.jpg)


---

### Artefatos - coleção de arquivos ou pacotes publicados por uma execução ( o produto do seu código )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’45”](https://user-images.githubusercontent.com/46926951/229640493-4ba7d54b-cbb0-4398-a15d-20ee4e88afcd.jpg)


---

### Configurar Pipeline com Yaml ( Starter Pipeline/não configurado e o Existing Azure/pré-configurado )


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’47”](https://user-images.githubusercontent.com/46926951/229879006-87b2fd5c-b179-4b19-8180-0633117e74a4.jpg)

---

### Usando o Starter Pipeline para criar o YAML

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’01”](https://user-images.githubusercontent.com/46926951/229879640-13d76eb4-d442-4ad6-a8a4-be83e8be2707.jpg)

> 1. Comentários

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’09”](https://user-images.githubusercontent.com/46926951/229879851-a80a30a3-d761-47ae-9d30-e78dfcf9a3e7.jpg)

---

> 2. Integração Contínua ( no exemplo da imagem abaixo, mostra o gatilho na branch Master, ou seja, sempre que a master for atualizada, irá executar esse pipeline  )

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’19”](https://user-images.githubusercontent.com/46926951/229880165-130f6c9d-a514-4371-8167-8a49edc6cf13.jpg)


---

> 3. Agent Pool ( Usa o agente hospedados pela Microsoft que utiliza o sistema operacional ubuntu-latest. Mas também pode utilizar outra, inclusive o Windows )

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’34”](https://user-images.githubusercontent.com/46926951/229880934-cdc29177-bca2-46c6-b248-5c74df44b81d.jpg)


---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’54”](https://user-images.githubusercontent.com/46926951/229881418-39d26eb6-cbc0-428e-8312-e331d5b1ae8c.jpg)


---


> 4. Steps ( Com scripts que escrevem no log uma mensagem e com displayName que é o nome do Step. E `echos` podem ser mais de um como na imagem )

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-4’06”](https://user-images.githubusercontent.com/46926951/229881880-783d9799-1d61-4176-bbf8-f593379fbd15.jpg)


---

- É importante lembrar que a formatação é importante. Sempre escrever a posição certa de cada linha.

---

> 5. Build iniciado e completado com sucesso ( depois de `commit` )

![image](https://user-images.githubusercontent.com/46926951/229883633-a5b4e1c9-1e35-4015-95f7-b71ed67ddeb0.png)

---

- Ele rodou os dois `steps` onde temos os scripts:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-7’09”](https://user-images.githubusercontent.com/46926951/229884122-92f201dc-58d1-4468-ad7c-e474797670dc.jpg)

---

### Schedule ( agendamento de builds )

- Padrão

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’28”](https://user-images.githubusercontent.com/46926951/229884969-17598057-3dec-4c04-8330-90296b1c387e.jpg)
---

- Agendamento ( seguindo o padrão acima, ele vai acionar às 10:35 minutos sempre (always =>  independente se houver alteração ou não no código) na branch master ( a do exemplo )

![image](https://user-images.githubusercontent.com/46926951/229885720-66d6928d-7332-4b95-bc74-2f2e6041a066.png)

---

### Jobs - Dependências e Condições

- Dependência: `dependsOn`. No caso da imagem abaixo, o `job1` dependerá do funcionamento do `job4`.
- Condição: `condition`. No caso da imagem, apenas se o `job4` falhar: `failed()`

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-9’44”](https://user-images.githubusercontent.com/46926951/229888146-25226804-a412-4782-8d93-c9380bb1acae.jpg)
---

- Exemplo com `succeeded:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-10’57” (1)](https://user-images.githubusercontent.com/46926951/229889124-31652103-452e-477d-bd15-1103d0dd915d.jpg)

---

### Stages de Jobs:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-5’23”](https://user-images.githubusercontent.com/46926951/229890949-beb888d3-c137-4181-b05e-b01eab74bead.jpg)

---

- Também pode ser utilizado dependsOn:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-17’22”](https://user-images.githubusercontent.com/46926951/229891312-877af735-eee6-4ec2-ab28-65698f4f527c.jpg)
---

### Tasks e Variáveis de Jobs\

![image](https://user-images.githubusercontent.com/46926951/229893276-b51fd781-ebcb-4d49-9283-7794d8ef6286.png)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-5’05”](https://user-images.githubusercontent.com/46926951/229893550-4a0924bd-41eb-4383-8bf1-31336e3180c6.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-5’29”](https://user-images.githubusercontent.com/46926951/229893761-d0229b7f-0d42-4de3-a693-b5a8d03494a2.jpg)

---

![image](https://user-images.githubusercontent.com/46926951/229894148-982e3c3a-3ad5-4d94-af0a-00a2efbda891.png)

---

## Princípios da Implantação Contínua ( CD = Continuos Deployment ) - implantação das alterações do código em produção

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’34”](https://user-images.githubusercontent.com/46926951/229897938-3dfe2975-3b73-4bf8-897e-deac209549f3.jpg)

---

---

## Princípios da Entrega Contínua ( CD = Continuos Delivery ) - 

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’51”](https://user-images.githubusercontent.com/46926951/229898414-69af2c5e-06ad-49b4-aced-3f274359f99a.jpg)

> 1. Processo Confiável Repetível: repetição do processo de implantação e confiança nele.
>
> 2. Automatize Tudo: automatizar tudo relacionado a implantação, teste de qualidade e segurança. Isso signfica menos esforço para executá-lo e monitorar o seu progresso garantindo resultados consistentes.
>
> 3. Repositório em Tudo: versionar a aplicação, configurações, infraestrutura, banco de dados e a documentação.
>
> 4. Mais complicado primeiro: lidar com as coisas difíceis primeiro. Tarefas demoradas ou propensas a erros devem ser tratadas primeiro e o mais rapidamente possível.
>
> 5. Qualidade Interna: criar `loops` de feedbacks curtos para lidar com `bugs` assim que ele forem criados.
>
> 6. Concluído significa liberado: aplicado apenas quando se está em produção.
>
> 7. Todos são responsáveis: a responsabilidade é de funcionamento em `todos` os ambientes ( local, hml, stage, prod ) e principalmente em produção.
>
> 8. Melhoria Contínua: O processo ser melhorado e revisado constantemente. Para isso é preciso monitorar e criar métricas.


## TDD - Test Driven Development ( desenvolvimento orietado a teste )
- teste unitário: é o componente principal desta metodologia

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’39” (1)](https://user-images.githubusercontent.com/46926951/229917069-e7a78faf-c343-4c5e-a03b-6e02ff58a874.jpg)

---

### Teste de Integração

- Avalia se a aplicação está funcionando como esperado através do consumo da api.
- Muito aplicado em API's Rest.
- Muito utilizado em arquiteturas de aplicação de microserviços.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’40”](https://user-images.githubusercontent.com/46926951/229917941-0a5d0bf6-af41-4927-8520-e4fe931dbcbc.jpg)

---

### Teste E2E ( End-to-End )

- Validar numa situação real como a aplicação irá se comportar.
- Também conhecido como testes automatizados.
- É o teste mais próximo de como o usuário interage com o aplicativo(simulando inputs, clicks e navegabilidade).
- Eles dependem do comportamento do UX. Isso significa que a interface esteja finalizada para uso.
- É uma estratégia mais lenta para a execução. 

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’28” (1)](https://user-images.githubusercontent.com/46926951/229918550-de032789-09b2-4741-99ae-a787e660a7cd.jpg)

---

- Ferramenta E2E mais utilizada para aplicativos web é o selênio

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’21”](https://user-images.githubusercontent.com/46926951/229920124-f70f13c1-cdd6-479c-97d4-120a4955c642.jpg)

---

##  Cloud - Escalonamento

> Scaling up

- O escalonamento vertical é botar mais capacidade de memória (principal e/ou de massa) e processamento. Ou seja, é comprar um hardware mais poderoso para dar conta do recado.

- Em alguns casos basta criar mais processos/threads que está fazendo o scaling up, desde que o hardware já suporte esse aumento. Há casos que separar o banco de dados em vários dispositivos de armazenamento já seja uma escala vertical, novamente é escalar na mesma máquina.

- O investimento é basicamente em hardware. Comprando mais processador. memória e armazenamento já tem uma capacidade aumentada.

- Em alguns casos é mais questão de fazer uma simples configuração para alcançar o que o hardware único já suporta.

- Também pode ser otimizar a aplicação para que ela desempenhe melhor e atenda mais do que fazia antes.

> Scaling out

- O escalonamento horizontal é colocar mais computadores para dar conta do recado. Claro que eles adicionam mais capacidade de processamento e memória também, na soma total.

- É muito mais complexo fazer um escalonamento horizontal tanto do ponto de vista de gerenciamento quanto do ponto de vista de programação, ainda que existam ferramentas para facilitar. Não é só colocar os computadores, eles precisam "se falar" de forma consistente e adequada. Na verdade isso é considerado o problemas mais difícil de resolver na computação.

- Por incrível que pareça pode ser mais barato que o vertical, pelo menos no custo da aquisição da infraestrutura já que é possível adquirir hardware mais simples e mais comum que costuma ser mais barato pela escala de produção. Claro que o custo de gerenciamento e desenvolvimento pode mudar o custo total.

- Fora os casos que o vertical não comportaria a necessidade, afinal essa estratégia tem um limite que em tese o horizontal não tem, o horizontal tem a vantagem de ser mais tolerante a falhas, ou pelo menos ser mais fácil ter a operação de volta em caso de alguma falha.

> Diferenças

- Qualquer banco de dados minimamente estruturado pode fazer os dois tipos de escalonamento. O vertical não precisa nenhuma propriedade específica a não ser no caso de separar dados em vários dispositivos de armazenamento ou permitir várias linhas de processamento, por isso não é simples fazer em certas modelagens. O horizontal precisa de mecanismos que permitam e, se possível, facilitem o escalonamento horizontal. Não importa se ele é do tipo não relacional ou não, se usa SQL ou não.

- Desconheço outros tipos, nem sei se é possível ter. Existem variações dessas formas, principalmente no horizontal existem muitas estratégias e técnicas. Também pode fazer um escalonamento híbrido.

- São raras as aplicações que precisam de escala horizontal. Pelo menos no sentido de escala mesmo. Pode ser útil fazê-lo pela confiabilidade maior de ter mais de um nó atendendo as requisições, mas não que precise de mais recursos. O grosso da necessidade vem de aplicações web de alta demanda ou processamentos muito específicos.

- Pode não parecer a mesma coisa mas tem uma pergunta que está relacionada, mostrando que escalar qualquer coisa horizontalmente pode parecer a solução, mas nem sempre resolve ou compensa a dificuldade que é inerente dela

### Exemplos

- Escalonamento Horizontal você adiciona mais máquinas em seu pool de recursos enquanto escalonamento Vertical significa que você adiciona mais poder (CPU, RAM) para uma máquina existente.

- Em um banco de dados Horizontal é muitas vezes baseada no particionamento dos dados, ou seja, cada nó contém apenas parte dos dados.

- No banco de dados Vertical os dados residem em um único nó (`node`) e o dimensionamento é feito através de multi-core, ou seja, espalha a carga entre o `CPU` e a `memória RAM`.

- No escalonamento horizontal muitas vezes é mais fácil de redimensionar dinamicamente adicionando mais máquinas, já na Vertical é muitas vezes limitada à capacidade de uma única máquina escalonar,além de que a capacidade muitas vezes envolve o tempo de inatividade e vem com um limite superior.

- Exemplo escalonamento horizontal: Cassandra, MongoDB..

- Exemplo escalonamento vertical MySQL - Amazon RDS (A versão nuvem de MySQL). Ele fornece uma maneira fácil de escalar verticalmente, passando de pequenos para máquinas maiores. Este processo envolve muitas vezes o tempo de inatividade.

- In-Memory Dados Grids como GigaSpaces XAP , Coerência etc .. são frequentemente otimizado tanto para escalonamento horizontal e vertical, simplesmente porque não é obrigado a disco. Horizontal através de particionamento e vertical através de apoio multi-core.

---

## Deployment Patterns - Estratégia de implantação

### 1. Big Bang ( também conhecida como Highlander, Reckless ou recreate )
- Padrão simples e básico de implantar.
- Este modelo apresenta vários problemas cujo principal é a indisponibilidade do sistema que é inevitável.
- Consistem em desligar a versão `A`:
![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’41”](https://user-images.githubusercontent.com/46926951/230180302-37bcb14b-69ba-4864-8169-027550819364.jpg)

---

- Para implantar a versão `B` depois que a `A` for desativada:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’44”](https://user-images.githubusercontent.com/46926951/230180799-463bdb82-0cfb-4da8-b9e1-d2d98f00f64c.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’53”](https://user-images.githubusercontent.com/46926951/230181649-ef09ffcf-f109-42de-8b15-34ed75aa725e.jpg)

---

### Onde usar e onde não-usar

> Não Usar Quando:

- Não são adequadas para `aplicativos modernos` porque os riscos são inaceitáveis voltados para o público externo.
- Não usar em aplicações críticas onde as interrupções representa enorme perda financeira.
- Pode-se usar `reversões` mas elas são muito demoradas, caras e até mesmo, algumas vezes, impossíveis de serem feitas. 

> Quando usar:

- Sistemas internos de baixa criticidade. Ex: recriar o ambiente de desenvolvimento.
- Sistemas de Desenvolvimento/Testes.
- Aplicativos de Desktop.
- Implantar apenas em agendas pré-determinadas: momentos com baixo acesso e na madrugada para minimizar o problema da indisponibilidade do sistema.

---

### 2. Implantação Ramped

- Implantação Gradual das versões `A` e `B`.
- Estratégia mais simples de ser adotada quando se quer um tempo mínimo de `Failover` (tolerância a falhas).
- É a utilizada por `default` nos serviços de `orquestração`.
- Ambas versões coexistem ao mesmo tempo em `produção` até a sua substituição completa que é feita gradualmente:

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’57”](https://user-images.githubusercontent.com/46926951/230184765-8bc73678-7c44-4417-98de-e7e597c57d42.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’00” (1)](https://user-images.githubusercontent.com/46926951/230185236-56af639c-3bf5-4097-8c22-f2746d552cae.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’00” (1)](https://user-images.githubusercontent.com/46926951/230185510-6e0a11c6-32a3-4715-bd2b-f009de5f2b9d.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’06” (1)](https://user-images.githubusercontent.com/46926951/230185763-b2ba6f42-cc8d-455b-8251-a5dffe3f65fc.jpg)

---

### Vantagens

- Monitorar a saúde do sistema: `Azure Monitor` e `Application Insides`.
- Rollback: proporciona a fácil reversão.
- Compatibilidade: entre a versão antiga e a nova.


### Indicações

- Sistemas com média criticidade e poucas atualizações.

- Ajuda do Serviço de Load Balancer do Azure para o Rollout ( lançamento ) e Rollback ( reversão ):

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’45”](https://user-images.githubusercontent.com/46926951/230187888-b608eed1-6983-4fec-ae8b-1c9bc2551c87.jpg)

--- 

### 3. Implantação Blue/Green

- Tipo de implantação de fases chamadas `blue` para `green`. Mas não é gradual como a ramped. Para este processo é usado o `swap`.
- Substitui completamente depois de testado e aprovado, uma versão do `blue` pela `green`.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’16” (1)](https://user-images.githubusercontent.com/46926951/230188637-20c1232c-1ec0-4257-b3ec-4a294ca7b748.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’22”](https://user-images.githubusercontent.com/46926951/230188914-bd3f9b47-d533-4be9-aead-2e84f6239b27.jpg)

---

- Utilizando o Swap:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’26”](https://user-images.githubusercontent.com/46926951/230189282-112e51a7-c605-4ff8-8fbc-b4b5aecde5b6.jpg)


### Vantagens

- Rollout e Rollback instantâneos: lançamento e reversão imediatas.
- Apenas uma versão: evita problemas como o `no-number` que é ter duas versoes simultâneas dividindo os usuários por algum tempo.
- Podem ser feitos testes em toda a plataforma na transferência do `blue` para o `green`.
- Ajuda do Serviço de Load Balancer do Azure para o Rollout ( lançamento ) e Rollback ( reversão ):

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’45”](https://user-images.githubusercontent.com/46926951/230187888-b608eed1-6983-4fec-ae8b-1c9bc2551c87.jpg)

----

### Desvantagens

- Dobro do recurso.
- Maior custo.
- Precisa-se de uma estrutura maior que a do modelo `ramped`.
- Perda de sessão: pode acontecer perda de dados durante o `deploy`.

---


### 4. Implantação Canary

- Nome dado por causa do uso de canários nas minas de carvão.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’30”](https://user-images.githubusercontent.com/46926951/230192867-46d1eadd-b384-49d5-beda-c5b1e40bb877.jpg)

---

- Os carvoeiros levavam o canário para dentro das minas. Ou seja, caso houvesse algum vazamento de gás, os canários morreriam primeiro.
- O canário era um teste. Se o canário morresse, o `teste` falhou.
- Neste caso, necessitariam fazer o `rollback` que era sair da mina dentro do contexto da história.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’53”](https://user-images.githubusercontent.com/46926951/230193582-0c815852-c308-47ab-ad8c-93eb2b7f36ea.jpg)

---

- O canary funciona como uma mitigação de risco. 
- São selecionados uma pequena quantidade de usuários do aplicativo para receber uma nova versão.
- E a sáude da aplicação é monitorado para estes usuários da nova versão(bugs ou erros do sistema).
- E se a saúde do sistema continuar estável, a nova versão é passada para os demais usuários.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’19” (1)](https://user-images.githubusercontent.com/46926951/230194972-6b08441a-69b8-419b-b2b6-045bc261a701.jpg)

---

- Pode ser usado geo-localização ou distribuir pelo `load balancer` determinando um percentual de usuarios para receber uma nova versão.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’49” (1)](https://user-images.githubusercontent.com/46926951/230196613-f0aae95c-18a7-46f9-8f6f-2916a020472d.jpg)

---

- O desafio da implantação de `canary` é conceber uma maneira de rotear alguns usuários para o `aplicativo`.
- Para isso se usa `slots` do `app server`: separando 90% para a produção(versão antiga) e 10% para o `canary`(versão nova).
- Outra possibilidade é expor usuários internos a implantação do `canary` antes dos usuários externos. Isso pode ser feito por `faixa de ip` através de `roteamento` baseado no intervalo de `ip de origem`.
- E pode ser utilizado o `azure-traffic-manager` nesta tarefa.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’49” (1)](https://user-images.githubusercontent.com/46926951/230196613-f0aae95c-18a7-46f9-8f6f-2916a020472d.jpg)

---

### 5. Implantação A/B Testing

- Trabalhando diferente do `canary`: os usuários não recebem uma nova versão para testar. Eles recebem variações para tal.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’20” (1)](https://user-images.githubusercontent.com/46926951/230199356-fd4dac3c-4ea4-457c-a990-b1c0001e21ef.jpg)


---

### Azure Traffic Manager

- Balanceador de tráfego baseado em `dns`.
- Oferece alta disponibilidade do sistema e capacidade de resposta.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’34”](https://user-images.githubusercontent.com/46926951/230199951-a60450ca-1e18-40fc-933a-b2c66b39af8d.jpg)

---

- Tipos de balanceamento para os `endpoints`:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’16”](https://user-images.githubusercontent.com/46926951/230200454-f9203540-aeaf-46de-ba82-4a581ee44f49.jpg)


---


## Kubernetes - k8s

- [DOC](https://kubernetes.io/pt-br/)

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’39”](https://user-images.githubusercontent.com/46926951/229922671-44dd2c6c-fbf9-4e76-ae66-ea0f92e5a3cc.jpg)

---

- Kubernetes é de origem grega e quer dizer `timoneiro`.
- É um sistema de código aberto para a orquestração de containers.
- Ele veio a existir depois de seu antecessor: o `borg`.


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’06”](https://user-images.githubusercontent.com/46926951/229923581-667a1e82-7364-487c-8301-bd154a9e7d2d.jpg)

---

### Plataformas CLOUD

- Na Amazon AWS o serviço do kubernetes é chamado de `eks`.
- Na Microsoft Azure é chamado de `aks`.
- No Google é chamado de `gke`.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’24”](https://user-images.githubusercontent.com/46926951/229932663-639eb8c3-264f-4eda-ada9-85922707b740.jpg)

---


### Kubernetes como orquestrador de containers

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’40”](https://user-images.githubusercontent.com/46926951/229924102-64c0427b-7654-4a18-a269-7cd953eea303.jpg)

---

- Ele é o responsável pela orquestração para a implantação, o gerenciamento e a escala de containers.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-4’45”](https://user-images.githubusercontent.com/46926951/229924657-3db80a2c-18be-43aa-9652-a17e840d464f.jpg)

---

### Arquitetura do Kubernetes

- [Componentes do Kubernetes](https://kubernetes.io/pt-br/docs/concepts/overview/components/)

> 1. Cluster
- Podemos ter um ou vários clusters 
- Qual é a função do cluster?

> O que é um cluster de Kubernetes?
>
> Um cluster de Kubernetes é um conjunto de nós(`nodes`) que executam aplicativos em `contêineres`. Os pacotes de aplicativos em contêineres contêm um aplicativo e alguns serviços necessários. Eles são mais leves e flexíveis que as máquinas virtuais. Dessa forma, os `clusters` de Kubernetes permitirão que os aplicativos sejam desenvolvidos, movidos e gerenciados mis facilmente.
>
> Os clusters de Kubernetes permitem que os contêineres sejam executados em várias máquinas e ambientes: virtuais, físicos, com base em nuvem e locais. Ao contrário das máquinas virtuais, os contêineres de Kubernetes não estão restritos a um sistema operacional específico. Em vez disso, eles podem compartilhar sistemas operacionais e ser executados em qualquer lugar.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-5’24”](https://user-images.githubusercontent.com/46926951/229926176-c7e94acc-b5ee-408f-86d0-43a53e317683.jpg)

---

- 1. A `Master`: é o ponto de controle central que possibilita a visão unificada do cluster. Ou seja, ela é a máquina mestre que recebe as configurações declaradas num arquivo `.yml`. É o mesmo formato de arquivo usado no `appliacation.yml` acima, como exemplo. E ela gerencia um ou mais `nodes`.

- 2. `Node`: é uma máquina ativa. E dentro dele ficam os serviços necessários para rodar os `pods`. Estes serviços são o `docker`, o `kubelet`, `cAdvisor`, `kubeproxy` ou `k-proxy`. Ele pode conter um ou mais `pods`.

- 3. `Pods`: é a menor unidade que pode ser criada, escalada ou manuseada. Funciona como uma coleção de `containers`. É um grupo de um ou mais `containers`, com armazenamento compartilhado e recursos de rede e uma especificação de como executar os contêineres. O conteúdo de um `pod` é sempre co-localizado e co-agendado e executado em um contexto compartilhado. Um Pod modela um `"host lógico"` específico do aplicativo: ele contém um ou mais contêineres de aplicativos que são relativamente fortemente `acoplados`. Em contextos fora da `nuvem`, os aplicativos executados na mesma máquina física ou virtual são análogos aos aplicativos em nuvem executados no mesmo host lógico. Assim como contêineres de aplicativos, um `pod` pode conter `contêineres init` que são executados durante a inicialização do pod. Você também pode injetar `contêineres efêmeros` para depuração se seu cluster oferecer isso. Ele pode conter um ou mais `containers`.

- 4. `Container`: o ideal é sempre usar um conteiner por `pod` por causa do `acoplamento`. É preciso manter um container por pod para manter o isolamento entre os containers, e assim cada um de seus recursos de memória e volume.

### Dentro disso tudo aí acima temos mais alguns componentes

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’06”](https://user-images.githubusercontent.com/46926951/229934138-4b0b7361-c8b3-42ce-8b16-1888c17c34d4.jpg)

---
> ETCD

- é o banco de dados.
- é o responsável pelo armazenamento de alta disponibilidade de informações.
- guarda as informações em formato chave e valores.
- armazena todos os dados de configurações e status do cluster.
- é usado como apoio para todos os dados de armazenamento do kubernetes.
- é preciso ter um plano de backup para estes dados.

- [DOC](https://etcd.io/)


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’07”](https://user-images.githubusercontent.com/46926951/229934063-49d56cf5-c99c-40e9-b34d-235a185898ab.jpg)

---

> Kube API Server

- Servidor de aplicações que fornece as `api's` do kubernetes por meio da teconologia `json`.
- Ele quem expõe a `api`.
- Os estados dos ojetos desse `applets` ficam armazenados no `ETCD`. e O `kubeCTL` usa o `Api Server` para se comunicar com o cluster.
- Ele pode ser dimensionado horizontalmente: implantação de mais instâncias e pode executar várias do `kube-api-server` e equilibrar o tráfego entre elas.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’09”](https://user-images.githubusercontent.com/46926951/229934332-6508e170-4cee-404f-962c-bece86125be7.jpg)

---

> Controller Manager

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’11”](https://user-images.githubusercontent.com/46926951/229934569-db446e16-9508-4612-b0eb-83152c886151.jpg)

---

> Worker Node

- é a representação em si: ele contém o `kubelet`, o `kubeproxy` e o `cAdvisor` e eles se conectam aos `pods` dentro do `docker`.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’12”](https://user-images.githubusercontent.com/46926951/229934779-919aa7e7-88fc-4c0c-a9d8-64ee0093d03c.jpg)

---

> Kube Scheduler

- Observa os `pods` recém-criados sem nenhum molde atribuído a eles e seleciona um `node` para executá-los. E faz isso levando em conta os requisitos de recursos individuais e coletivos, restrições de hardware, software e política. Além de especificações de afinidades e anti-afinidades, localidade de dados, interferência entre carga de trabalho e seus prazos.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’13”](https://user-images.githubusercontent.com/46926951/229934899-fcced78c-c2c9-48a3-b83c-ac32f6a491b7.jpg)

---

> KubeCTL

- O `kubeCTL` usa o `Api Server` para se comunicar com o cluster.
- Ele é uma ferramenta de linha de código para se comunicar com o `Kube API Server`.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’15”](https://user-images.githubusercontent.com/46926951/229934995-d22181ff-e3f2-4ace-8da2-071690ddd494.jpg)

---

> Kubelet

- é o agente executado em cada um dos `nodes` de um worker quando ele se conecta ao `docker`.
- ele tem a responsabilidade de realizar a criação, modificação, execução e exclusão dos containers.
- ele obtém informações da `master` e garante que todos os `pods` atribuídos a ele estejam em execução e configurados em seu estado desejado.
- todos os `nodes` do `kubernetes` deve ter um `Kubelet`.
- ele cria um `pod` deixando-o pronto para o `container`.
- testa e verifica a saúde do `container`.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’16”](https://user-images.githubusercontent.com/46926951/229935105-f4ebbfa1-87d6-4c63-b8f3-a4bde614ac5b.jpg)

---

> Kubeproxy

- observa todos os serviços e mantém a configuração da rede em todos os elementos do `cluster`.
- ele faz isso encaminhando os tráfegos para os `containers` com base nos endereçamentos dos `ip's` e nos números das `portas` da solicitação processada.
- 

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’17” (1)](https://user-images.githubusercontent.com/46926951/229935179-c12d7ad7-3c1d-432d-a678-657202f12ebc.jpg)


---

> Replication Controller

- Responsável por manter o número correto de `pods` para cada objeto de `controller` e replicação no sistema.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’19”](https://user-images.githubusercontent.com/46926951/229935285-7c318f47-2a6b-418d-9457-79ebe503a874.jpg)

---


> Services Controller

- são criadas contas padrões e tokens de acesso a `api` para novos ingressantes.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’20”](https://user-images.githubusercontent.com/46926951/229935367-c49ae603-8b8e-45cd-83c0-d57117ff0a09.jpg)

---


> cAdvisor 

- O `cAdvisor` é um agente de código aberto integrado ao binário `kubelet` que monitora o uso de recursos e analisa o desempenho dos `contêineres` . 
- Ele coleta estatísticas sobre o uso de `CPU`, `memória`, `arquivo` e `rede` para todos os contêineres em execução em um determinado `node` ( não opera no nível do `pod` ).
- É também o responsável por coletar métricas sobre os `pods` em execução para o `node`.

![image](https://user-images.githubusercontent.com/46926951/230130586-4d4a9443-fe43-4495-bee4-02be37225b49.png)

---

> Pod

- Um grupo de containers implantados em um único Worker Node
- Ele é um conceito crucial no `kubernetes`.
- É o ponto os `desenvolvedores` interagem.
- É a menor unidade no `cluster` de kubernetes.
- Nele é rodado o `container`.
- Roda um ( o ideal ) ou mais de um `container` dentro dele. Com isso compartilha recursos e instruções sobre como executar o container. 


![image](https://user-images.githubusercontent.com/46926951/230132989-b1bd71ad-2204-47c9-a0d2-32797478402e.png)

---

- Os pods podem se comunicar dentro do `cluster` usando o `ip` de serviço.


![image](https://user-images.githubusercontent.com/46926951/230138074-fba04c70-a5d5-4646-b5b9-1e4716f12367.png)

---

> 1° Pod => contém um `aplicativo` em `container`.
>
> 2° Pod => contém um `aplicativo` em `container` e o seu `volume`.
>
> 3° Pod => contém dois `aplicativos` em `containers` e um `volume`.
>
> 4° Pod => contém três `aplicativos` em `containers` e dois `volumes`. O seu uso, para melhor compreensão são: aplicações onde podemos ter mais de um aplicativo integrado `verticalmente`. Por exemplo, uma aplicação `Wordpress`: onde tem um `servidor Linux`, e dentro dele tem um `servidor Web` do tipo `Apache`. Um `banco de dados` do tipo `Mysql`, e uma aplicação em `PHP` rodando no `Wordpress`.
- Nos casos acima, é notório perceber o compartilhamento do endereço de `ip` e o seu `volume` dentro deste `pod`.
- Os `pods` não são `imortais`, eles morrem. Ou seja, possuem uma vida útil limitada. Isso acontece se a sua escala for reduzida ou quando a versão sofre alguma atualização.
- Eles possuem a habilidade de realizar dimensionamento horizontal(com isso aumenta ou diminui o número de instâncias) e também pode realizar o `deploy`.
- Deploy Pattern a ser levada em consideração, é a do tipo `Canary`. Com isso, existem vários tipos de `pods`. Sendo o `default`, o réplica 7. Cujo o objetivo desse, é manter um conjunto estável de `pods` de réplicas em execução a qualquer momento. Assim ele garante a disponibilidade de números específicos de `pods` idênticos.
- O `pod deployment` é uma forma decorativa de gerenciar `pods` por meio de réplicas 7. Ele inclui mecanismos de reversão e atualização contínua. E onde também é declarada o tipo de implantação que será feita do tipo `canary`.
- No `pod deployment` é declarado o que precisamos. E o `deployment controller` o executa.

---
- Exemplo do `deployment`. Criação do `réplica 7` para três `pods`:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-7’16”](https://user-images.githubusercontent.com/46926951/230153223-77b316c3-12e3-4898-8bff-1867dafe873f.jpg)


---

> Container

- Ele roda dentro do `pod`.
- O ideal é rodar um container por `pod`. Mas podem `rodar` mais de um dentro desse.


![image](https://user-images.githubusercontent.com/46926951/230136226-a42e8ea9-8394-48a9-a3c2-39f5176dc5d0.png)



---


### kubernetes Control Plane e o Kubernetes Node

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-9’07”](https://user-images.githubusercontent.com/46926951/230174193-97da7ae0-c7f5-4ec8-8542-03a4b0a7c603.jpg)

> Controllers

- 1 - `Kube-Controller Manager`: componente do `Master` e roda os controladores.
- `node controller`: responsável por modificar e responder quando e como os `nodes` caem.

- 2 - `Cloud-Controller Manager`: permite que o código do fornecedor de `cloud` e o código do `kubernetes` possam evoluir independentes um do outro.

- Endpoints: fazem a junção dos serviços e `pods`.



### Preciso do Kubernetes?
- Se a resposta for `sim` para uma ou para as duas perguntas, é necessário utilizar:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’58”](https://user-images.githubusercontent.com/46926951/229931478-f8d1e19f-3287-4e80-83ad-5d1347f1587b.jpg)

---

### Recursos do Kubernetes
- Só faz sentido se a aplicação opera com poucos usuários
- Trabalhando com Microserviços, é essencial trabalhar com k8s.
- Fundamental para um sistema que necessita ficar no `ar` em pleno funcionamento e tem `picos de acesso` constantes.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’46”](https://user-images.githubusercontent.com/46926951/229931794-acd3d0c2-d587-4e01-8876-a3bfcc01a0b4.jpg)

---

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’03”](https://user-images.githubusercontent.com/46926951/229932473-d65edb64-d9d8-45c9-b64a-b6ce0e1595ec.jpg)

---


### K8s Tem serviço de portabilidade entre os serviços

- 


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’24”](https://user-images.githubusercontent.com/46926951/229932663-639eb8c3-264f-4eda-ada9-85922707b740.jpg)

---


### K8s Usado também no Machine Learning e Big Data

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’40”](https://user-images.githubusercontent.com/46926951/229933223-d63765d8-3dd8-4988-8c20-4ffd81c6d656.jpg)

---

### Kubernetes também usado em soluções `servless` como o Knative

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’53”](https://user-images.githubusercontent.com/46926951/229933407-7484ff66-e508-4c35-9718-9eb83747755c.jpg)

---

## Infraestrutura em Código (IaC)

- E o maior desafio é mudar a `cultura` e diminuir a curva de aprendizagem.

- A `antiga` cultura é baseado no modelo `humano` para provisionar ambientes. E este movimento de infraestrutura como código (IaC) veio para mudar porque traz consigo a cultura `nova` onde tudo é versionado e automatizado eliminando clicks e mais clicks.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’32”](https://user-images.githubusercontent.com/46926951/230663676-0e5573af-ebae-4a63-b074-836f5be21de7.jpg)

---

#### Vantagens:

- Provisionar recursos utilizando `scripts` é possível trazer a `infraestrutura` cada vez mais próxima do `desenvolvimento`. E também o desenvolvimento mais próximo da infraestrutura. E isso torna a cultura `DevOps` mais forte nos times da empresa.

- Entrega de ambientes cada vez mais rápidos. A automação da `infra` através do `IaC`, acelera o processo de provisionamento tanto na criação de ambientes de desenvolvimento, de testes e até mesmo de produção.

- Eliminação de documentos e manuais. A `infra` está no código.

- A `infraestrutura` não fica dependente de `donos`. Até o `dev` pode escrever como precisa desta `infraestrutura`.

- Podem ser criados `testes` sobre a infraestrutura.

- A IaC pode ser adicionada nas Pipelines.

---

### Ferramentas

- Scripts em `PowerShell` ou `Bash`.

---

### Ferramentas para a ação
- Mais usadas são o `Terraform` ou `Ansible`

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’59” (2)](https://user-images.githubusercontent.com/46926951/230664046-16d1fc47-cf92-4fe2-9868-71c1fb8aa775.jpg)

---

#### ARM ( Azure Resource Manager )

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’24”](https://user-images.githubusercontent.com/46926951/230664286-242a5c04-2f83-4197-85cc-b628c7a128e2.jpg)

---

- Criação de scripts a partir do portal do próprio `Azure`.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’18”](https://user-images.githubusercontent.com/46926951/230666115-007815bb-784e-4196-807b-220a30d89a06.jpg)

---

### Ferramentas do ARM

- Templates prontos que podem ser utilizados:

[ Azure Resource Manager - Quick Starts - templates prontos ](azure.microsoft.com/pt-br/resources/templates)

- Templates também podem ser criados no VSCode:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’58”](https://user-images.githubusercontent.com/46926951/230667107-5aea8b29-c36e-4555-b7e5-d787dbaa199a.jpg)

---

- Com este plugin, é possível visualizar o ARM em formato de `diagrama`: 

[ Plugin ARM Template Viewer - Plugin do Visual Studio Code ](marketplace.visualstudio.com/items?itemName=bencoleman.armview)

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’01”](https://user-images.githubusercontent.com/46926951/230666518-d6614cef-d7b6-4830-adf0-437dff68ab82.jpg)

---

- Plugin de autocomplete para criar os scripts:

[Plugin Azure Resource Manager (ARM) Tools - auto-complete - Plugin do Visual Studio Code](marketplace.visualstudio.com/items?itemName=msazurermtools.azurerm-vscode-tools)


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’30” (1)](https://user-images.githubusercontent.com/46926951/230667837-3d3bd5e7-733d-4565-972a-99e8c9a319aa.jpg)


---

#### Terraform

- Ferramenta declarativa de provisionamento e orquestração de infra-estrutura que permite ao time automatizar o provisionamento de todos os aspectos de sua infraestrutura corporativa.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’36”](https://user-images.githubusercontent.com/46926951/230668455-b96e21da-40de-49b2-84b7-ac599adb7707.jpg)


--- 


- Baseado na nuvem e também com o primes. Ele pode ser utilizado também no `aws` e Google Cloud Plataform:


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’01”](https://user-images.githubusercontent.com/46926951/230668933-36f8976e-090b-4372-abf0-74b58fd38b26.jpg)


---

- Ele trabalha com todos os principais provedores de nuvem e permite automatizar a criação de recursos em vários provedores em paralelo, independente de onde residem os servidores físicos, os servidores de `DNS` ou o do `banco de dados`, e essa é a maior vantagem dessa ferramenta. Uma única ferramenta que pode ser utilizada com qualquer grande provedor da nuvem.


- Pode fornecer qualquer aplicativos escritos em qualquer linguagem e seu uso é ainda mais simples que o ARM.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’52”](https://user-images.githubusercontent.com/46926951/230669802-62910841-c824-48a3-9e4c-308662e557b2.jpg)


---


- Não oferece recursos de gerenciamento de configuração como outras ferramentas. Como por exemplo, o `Ansible`. Mas pode trabalhar lado-a-lado com elas.

- A linguagem própria do Terraform é chamada de `hcl` ( sigla: hashicorp configuration language ). É uma linguagem `concisa` e `legível`( mais legível que o `json` usado no `arm`).

- Com o `hcl` é possível `criar` e `descrever` toda a infraestrutura usando uma sintaxe declarativa.

- Ele é `multi-provider`.

- A curva de aprendizado é baixo.

---

## Devops Databases

- Deve fazer parte da CD ( `entrega contínua` - continuos delivery )


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-2’02”](https://user-images.githubusercontent.com/46926951/230672077-0113c582-03d0-4974-b773-f05f0cdd4b42.jpg)


---

- Adicionar o banco de dados é super importante na esteira de DevOps:

> O que é esteira em desenvolvimento?
>
> Uma esteira tradicional que segue os conceitos da agilidade é chamada de SDLC — sigla para Software Development Life Cycle, literalmente traduzido como `Ciclo de Vida de Desenvolvimento de Produto`.


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-5’04”](https://user-images.githubusercontent.com/46926951/230672996-58c8457c-7ee1-4c1f-9cce-066b76c22df6.jpg)


---

#### Desafios

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-6’20”](https://user-images.githubusercontent.com/46926951/230673269-f8f19ecb-ae1b-40ce-a8b0-dac372e158c0.jpg)


---


- O DBA precisa estar junto na CI ( implantação contínua - Continuos Integration ), ou seja, ele precisa ser incluído na cultura `DevOps`.


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-7’16” (1)](https://user-images.githubusercontent.com/46926951/230673149-1334848b-69d5-49ae-8273-6826cd660ac8.jpg)


## Flyway




