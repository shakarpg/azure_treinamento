# Azure AZ 900 Treinamento - Aprendizado e Práticas

Este repositório contém todos os recursos, exercícios e anotações do treinamento sobre **Microsoft Azure** que você fez. O objetivo aqui é consolidar o conhecimento adquirido e documentar as práticas realizadas durante o processo de aprendizado.

---

## Índice
- [Introdução ao Azure](#introdução-ao-azure)
- [Gerenciamento de Recursos](#gerenciamento-de-recursos)
- [Configuração de Máquinas Virtuais](#configuração-de-máquinas-virtuais)
- [Redes Virtuais e Sub-redes](#redes-virtuais-e-sub-redes)
- [Monitoramento e Segurança no Azure](#monitoramento-e-segurança-no-azure)
- [Automação no Azure](#automação-no-azure)
- [Referências e Links Importantes](#referências-e-links-importantes)

---

## Introdução ao Azure

Durante o treinamento, aprendemos os conceitos fundamentais sobre **Microsoft Azure**, a plataforma de nuvem da Microsoft. Alguns dos principais tópicos abordados foram:

- **O que é o Azure?**
  - Uma plataforma de computação em nuvem pública que oferece uma gama de serviços como computação, armazenamento, rede e bancos de dados.
  
- **Principais benefícios do Azure**
  - Escalabilidade
  - Segurança avançada
  - Flexibilidade para trabalhar com diferentes tecnologias

- **Criação de uma conta no Azure**
  - Como criar uma conta no [Microsoft Azure](https://azure.microsoft.com/).

![Criação de Conta Azure](images/criacao-conta-azure.png)
> *Exemplo da criação de conta no Azure.*

---

## Gerenciamento de Recursos

Uma das primeiras coisas que aprendemos foi como gerenciar os **recursos no Azure**. Aqui estão alguns dos pontos abordados:

- **Criação de grupos de recursos**
  - Como criar e organizar recursos dentro de grupos de recursos no portal Azure.
  
- **Gerenciamento de Assinaturas**
  - Como configurar e gerenciar diferentes assinaturas para diferentes ambientes (produção, desenvolvimento, etc).
  
- **Uso do Azure CLI**
  - Comandos básicos do [Azure CLI](https://docs.microsoft.com/pt-br/cli/azure/).

  ## Configuração de Máquinas Virtuais

Uma das tarefas mais práticas foi aprender a configurar Máquinas Virtuais (VMs) no Azure. Durante este processo, vimos:

**Criando uma VM via Azure Portal**

Como criar uma máquina virtual usando o portal Azure, escolhendo a imagem do sistema operacional, tamanho e configuração.

**Configuração via Azure CLI**

Aprendemos a criar e configurar uma VM via linha de comando com o comando abaixo:

az vm create --resource-group MeuGrupoDeRecursos --name MinhaVM --image UbuntuLTS --size Standard_B1s

[imagem vm](,/img/)

**Conexão remota com a VM**

Como acessar a VM via SSH e configurar segurança e atualizações.

Exemplo de uma máquina virtual configurada no Azure.

**Redes Virtuais e Sub-redes**

Outro ponto importante foi a configuração de Redes Virtuais (VNets) e Sub-redes no Azure, essencial para gerenciar a comunicação segura entre os recursos.

**Criação de uma VNet:**

A VNet permite a comunicação privada entre as máquinas virtuais e outros recursos do Azure.

az network vnet create --name MinhaVNet --resource-group MeuGrupoDeRecursos --subnet-name MinhaSubrede


**Configuração de sub-redes e grupos de segurança de rede (NSG):**

Como configurar regras de tráfego de rede para controlar o acesso às máquinas virtuais e outros recursos.

Exemplo de configuração de rede virtual no Azure.

**Monitoramento e Segurança no Azure**

Um dos tópicos mais importantes foi como monitorar e garantir a segurança dos recursos no Azure.

**Azure Monitor e Azure Security Center**

Como usar o Azure Monitor para acompanhar a performance e saúde dos recursos.

Azure Security Center para proteger os recursos, detectar vulnerabilidades e ameaças.

Tela de monitoramento de recursos no Azure.


## Automação no Azure

Por fim, um dos aprendizados mais interessantes foi a Automação no Azure. Utilizamos o Azure Automation para automatizar tarefas repetitivas.

**Automação com Runbooks**

Criamos Runbooks (scripts) no Azure Automation para executar tarefas como backups, atualizações e manutenção de recursos automaticamente.

az automation runbook create --resource-group MeuGrupoDeRecursos --automation-account-name MinhaContaDeAutomacao --name MeuRunbook --type PowerShell


Usando Logic Apps para integrar serviços:

Aprendemos a integrar diferentes serviços e fluxos de trabalho usando Logic Apps, que permitem orquestrar tarefas de maneira visual.

Exemplo de automação utilizando Logic Apps.


##  Conclusão

O treinamento foi fundamental para entender a infraestrutura de nuvem do Azure e como gerenciar recursos, máquinas virtuais, redes e automação de processos. Agora, você pode utilizar essas habilidades para otimizar seu trabalho na nuvem, além de integrar as melhores práticas de segurança e monitoramento.

```bash
az group create --name MeuGrupoDeRecursos --location brazilsouth
