## 🚚 Sistema Automatizado de Fluxo e Gestão de Frotas

#📌 Sobre o Projeto
Este projeto foi desenvolvido para resolver um problema real de **Silos de Informação** entre departamentos, para qualquer empresa em rápido crescimento. O sistema centraliza a entrada de dados de campo e automatiza a passagem de bastão (*Hand-off*) entre os departamentos técnico, frotas, diretoria e financeiro, reduzindo o tempo de ociosidade de veículos parados em manutenção (SLA).

#🛠️ Tecnologias e Ferramentas Utilizadas
* Microsoft Forms: Interface amigável para coleta de andamentos operacionais.
* Microsoft Power Automate (Workflow): Motor de integração que grava os dados e gerencia a lógica de distribuição de alertas por e-mail utilizando o controle condicional de cenários (`Switch/Opção`).
* Excel Online (OneDrive): Arquitetura de banco de dados relacional dividida em tabelas de Dimensão (Cadastro) e Fato (Histórico Cronológico).
* Visão Geral de Dados via Forms: Painel de monitoramento com gestão à vista baseado nos dados das informações inseridas no formulário. É possível criar um relatório executivo no Power BI.

#🔄 Fluxo de Funcionamento (Arquitetura)
1. O time técnico/estagiários insere um andamento de veículo no *Forms*.
2. O Power Automate captura a resposta em tempo real.
3. Os dados são inseridos na tabela de histórico cronológico em nuvem.
4. O sistema avalia o responsável atual e dispara um e-mail inteligente direcionado (ex: enviando para a Diretoria casos de alçada alta, ou para o Analista para execução técnica) com o link de retorno do fluxo.

#📁 Como Utilizar este Repositório
* Na pasta `/database` você encontra a base de dados realista com 100 linhas utilizada para testes de relacionamento (1:*) de dados.
* Na pasta `/automations` está disponível o arquivo de importação do pacote ZIP do Power Automate para replicação do fluxo em outros ambientes do Office 365.

#🛠️ Tecnologia Utilizada
**Microsoft Excel**
- Power Automate / Forms / OneDrive / Outlook.
- Arquivos incluídos neste repositório: Arquivo `.zip` da fiação lógica do Power Automate e a base simulada em formato Excel.

#📊 Prints do Projeto:

<img width="1919" height="911" alt="print-01" src="https://github.com/user-attachments/assets/d7c0b81a-83dc-4a6b-894c-a95c64216439" />

<img width="1919" height="909" alt="print-02" src="https://github.com/user-attachments/assets/4d5f3016-8e9b-457c-acc1-eec3a777b84d" />

<img width="1919" height="908" alt="print-03" src="https://github.com/user-attachments/assets/1b06f762-e3a8-4f6b-a9bb-7eb42fd2ac50" />

<img width="1919" height="911" alt="print-04" src="https://github.com/user-attachments/assets/9e213ffc-9b4f-4e4b-ab84-9efd8800d9a2" />

<img width="1919" height="911" alt="print-05" src="https://github.com/user-attachments/assets/cfd53506-8559-42bd-af48-f3cb0af35af6" />

<img width="1918" height="909" alt="print-06" src="https://github.com/user-attachments/assets/b29de8b7-b117-4a0d-97aa-4168816dae81" />

<img width="1919" height="908" alt="print-07" src="https://github.com/user-attachments/assets/ec9a54c1-b879-4a1e-b470-f716c40dc485" />

<img width="1919" height="912" alt="print-08" src="https://github.com/user-attachments/assets/f7e45d2f-240e-40a3-81d1-e0d5d6de6cb3" />

<img width="1919" height="910" alt="print-09" src="https://github.com/user-attachments/assets/865bf937-4d31-4c8d-80db-8983205ea909" />
