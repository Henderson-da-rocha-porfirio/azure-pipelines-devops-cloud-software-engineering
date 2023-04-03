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
