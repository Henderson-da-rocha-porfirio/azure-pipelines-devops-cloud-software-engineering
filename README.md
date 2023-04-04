# azure-pipelines-devops-engineering

### Muito mais que ferramenta, é cultura!

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

### Kubernetes - k8s

- [DOC](https://kubernetes.io/pt-br/)

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’39”](https://user-images.githubusercontent.com/46926951/229922671-44dd2c6c-fbf9-4e76-ae66-ea0f92e5a3cc.jpg)

---

- Kubernetes é de origem grega e quer dizer `timoneiro`.
- É um sistema de código aberto para a orquestração de containers.
- Ele veio a existir depois de seu antecessor: o `borg`.


![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-3’06”](https://user-images.githubusercontent.com/46926951/229923581-667a1e82-7364-487c-8301-bd154a9e7d2d.jpg)

---

### Plataformas CLOUD

- Na AWS o serviço do kubernetes é chamado de `eks`.
- No Azure é chamado de `aks`.

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
> Um cluster de Kubernetes é um conjunto de nós que executam aplicativos em contêineres. Os pacotes de aplicativos em contêineres contêm um aplicativo e alguns serviços necessários. Eles são mais leves e flexíveis que as máquinas virtuais. Dessa forma, os clusters de Kubernetes permitirão que os aplicativos sejam desenvolvidos, movidos e gerenciados mis facilmente.
>
> Os clusters de Kubernetes permitem que os contêineres sejam executados em várias máquinas e ambientes: virtuais, físicos, com base em nuvem e locais. Ao contrário das máquinas virtuais, os contêineres de Kubernetes não estão restritos a um sistema operacional específico. Em vez disso, eles podem compartilhar sistemas operacionais e ser executados em qualquer lugar.

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-5’24”](https://user-images.githubusercontent.com/46926951/229926176-c7e94acc-b5ee-408f-86d0-43a53e317683.jpg)

---

- 1. A `Master`: é o ponto de controle central que possibilita a visão unificada do cluster. Ou seja, ela é a máquina mestre que recebe as configurações declaradas num arquivo `.yml`. É o mesmo formato de arquivo usado no `appliacation.yml` acima, como exemplo. E ela gerencia um ou mais `nodes`.

- 2. `Node`: é uma máquina ativa. E dentro dele ficam os serviços necessários para rodar os `pods`. Estes serviços são o `docker`, o `kubelet` e `kubeproxy` ou `k-proxy`. Ele pode conter um ou mais `pods`.

- 3. `Pods`: é a menor unidade que pode ser criada, escalada ou manuseada. Funciona como uma coleção de `containers`. É um grupo de um ou mais `containers`, com armazenamento compartilhado e recursos de rede e uma especificação de como executar os contêineres. O conteúdo de um `pod` é sempre co-localizado e co-agendado e executado em um contexto compartilhado. Um Pod modela um `"host lógico"` específico do aplicativo: ele contém um ou mais contêineres de aplicativos que são relativamente fortemente `acoplados`. Em contextos fora da `nuvem`, os aplicativos executados na mesma máquina física ou virtual são análogos aos aplicativos em nuvem executados no mesmo host lógico. Assim como contêineres de aplicativos, um `pod` pode conter `contêineres init` que são executados durante a inicialização do pod. Você também pode injetar `contêineres efêmeros` para depuração se seu cluster oferecer isso. Ele pode conter um ou mais `containers`.

- 4. `Container`: o ideal é sempre usar um conteiner por `pod` por causa do `acoplamento`. É preciso manter um container por pod para manter o isolamento entre os containers, e assim cada um de seus recursos de memória e volume.


### Preciso do Kubernetes?
- Se a resposta for `sim` para uma ou para as duas perguntas, é necessário utilizar:

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-0’58”](https://user-images.githubusercontent.com/46926951/229931478-f8d1e19f-3287-4e80-83ad-5d1347f1587b.jpg)

---

### Recursos do Kubernetes
- Só faz sentido se a aplicação opera com poucos usuários

![VideoScreenshot--AzurePipelines-CICDDockereKubernetesnoAzureDevOpsUdemy-1’46”](https://user-images.githubusercontent.com/46926951/229931794-acd3d0c2-d587-4e01-8876-a3bfcc01a0b4.jpg)





























