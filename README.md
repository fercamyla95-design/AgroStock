# AgroStock

### Controle e rastreabilidade de estoque de insumos agrícolas

Projeto desenvolvido a partir de uma solução utilizada na operação da Fazenda Triângulo para organizar o controle de retirada, devolução e movimentação de produtos agrícolas.

O sistema utiliza **QR Code + Google Forms + Excel**, permitindo registrar as movimentações diretamente pelo celular e posteriormente organizar essas informações em uma planilha de controle.

---

## 📌 Sobre o projeto

O AgroStock nasceu de uma necessidade prática:

> Como registrar de forma simples quem retirou um produto, qual produto foi retirado, em que quantidade e para qual área ele foi destinado?

Antes da implementação, parte dessas informações precisava ser registrada e organizada manualmente.

A solução criada utilizou um **QR Code fixado no local de armazenamento dos produtos**. Ao escanear o código pelo celular, o responsável era direcionado para um formulário onde informava os dados da movimentação.

### Fluxo da operação

```text
📱 Celular
     ↓
📷 Leitura do QR Code
     ↓
📝 Google Forms
     ↓
📊 Registro das respostas
     ↓
📋 Planilha de controle
     ↓
📦 Controle de estoque

🚜 Aplicação na operação
O sistema foi utilizado durante aproximadamente 5 meses, incluindo o período de safra e colheita da soja.
Durante esse período, o processo passou por ajustes e melhorias conforme as necessidades observadas na operação.
O objetivo principal era tornar o registro das movimentações mais simples e melhorar a rastreabilidade dos produtos.

📷 QR Code utilizado
O QR Code foi colocado próximo ao local de armazenamento dos produtos.
Ao realizar a leitura, o usuário acessava o formulário utilizado para registrar a movimentação.

O aviso na imagem orientava:
Retirada de Produtos
Escanear QRCode e Responder Formulário

Essa abordagem eliminou a necessidade de procurar manualmente o formulário e facilitou o registro diretamente no local da operação.

📝 Formulário utilizado
O formulário era utilizado para registrar as movimentações dos produtos.
Entre as informações registradas estavam:
- Produto;
- Quantidade;
- Entrada ou saída;
- Destino / talhão;
- Responsável pela movimentação;
- Data e horário do registro;
- Outras informações necessárias para o controle.
O formulário atualmente não está mais em operação e é disponibilizado apenas como referência/documentação do projeto.
Formulário utilizado

🔗 Acessar o formulário utilizado como referência
Observação: o formulário foi desativado para utilização operacional. O link é mantido no projeto apenas para demonstrar como funcionava a solução.

📊 Visualização das respostas
O Google Forms disponibilizava uma área de respostas com gráficos e resumos das informações registradas.
Essa visualização permitia acompanhar de forma rápida os produtos e quantidades informados nos registros.

O acesso aos gráficos e à visualização das respostas era restrito aos administradores do formulário.

📦 Controle em Excel
As informações registradas pelo formulário eram utilizadas como base para alimentar a planilha de controle operacional.
A planilha possuía diferentes áreas para organização das informações, incluindo:
Estoque e cadastro
Controle dos produtos cadastrados, unidades de medida e estoque atual.
Entradas

Registro de produtos recebidos, incluindo informações como:
- Código do produto;
- Data de entrada;
- Quantidade;
- Origem;
- Fornecedor;
- Descrição do produto;
- Unidade de medida.
Saídas

Registro das retiradas dos produtos, incluindo:
- Código do produto;
- Data da saída;
- Quantidade;
- Responsável;
- Destino / talhão;
- Produto;
- Unidade de medida.

Dessa forma, era possível relacionar:
produto → quantidade → data → responsável → destino
proporcionando maior rastreabilidade das movimentações.

🗂️ Estrutura do projeto
AgroStock/
│
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
│
├── data/
│   └── sample/
│       └── movimentacoes_exemplo.csv
│
├── docs/
│   ├── fluxo.md
│   ├── projeto.md
│   └── images/
│       ├── qr-code-operacao.jpg
│       ├── graficos-respostas-formulario.png
│       └── graficos-respostas-formulario2.png
│
└── src/
    └── preparar_movimentacoes.py

🛠️ Tecnologias e ferramentas
- Google Forms — coleta das informações;
- QR Code — acesso rápido ao formulário;
- Microsoft Excel — controle e organização do estoque;
- Python / Pandas — preparação e tratamento de dados para futuras evoluções;
- GitHub — documentação e versionamento do projeto.

🔒 Privacidade dos dados
Por se tratar de um projeto baseado em uma operação real, os dados publicados neste repositório foram adaptados para fins de demonstração.
Alterações realizadas
- Nomes pessoais foram substituídos por identificadores genéricos:
  - Responsável 1
  - Responsável 2
  - Responsável 3
  - etc.

- A mesma pessoa mantém o mesmo identificador ao longo dos arquivos;
- Dados reais de identificação pessoal não são disponibilizados;
- Os dados utilizados para demonstração pública foram tratados para evitar exposição de informações pessoais.
Os nomes de locais utilizados na operação foram mantidos quando não representam informações pessoais ou endereços.

📊 Dados de demonstração
Os arquivos disponibilizados neste projeto têm como objetivo demonstrar a estrutura e o funcionamento da solução.
Quando necessário, os dados foram anonimizados ou substituídos por registros de demonstração.
A intenção é permitir que outras pessoas compreendam a lógica do projeto sem expor informações pessoais da operação original.

💡 O que o projeto demonstra
Mais do que um simples controle de estoque, o AgroStock demonstra a aplicação de tecnologia para resolver um problema real de uma operação agrícola.
O projeto envolve:
- Identificação por QR Code;
- Coleta de dados pelo celular;
- Padronização dos registros;
- Controle de entradas e saídas;
- Rastreabilidade de movimentações;
- Organização de dados;
- Utilização de planilhas para apoio à gestão;
- Identificação de oportunidades para automação.

🚀 Próximos passos — AgroStock 2.0
A primeira versão teve como foco resolver o problema operacional e validar o processo na prática.
Uma próxima etapa poderá evoluir a solução para uma estrutura mais automatizada, utilizando:
- Python;
- Pandas;
- Banco de dados;
- Dashboard;
- Atualização automática do estoque;
- Relatórios;
- Indicadores;
- Histórico de movimentações;
- Alertas de estoque;
- Integração entre coleta e controle;
- Análises para apoio à tomada de decisão.

Essas funcionalidades fazem parte de uma possível evolução futura do projeto e não devem ser confundidas com o sistema originalmente utilizado na operação.

🎯 Objetivo do projeto
O AgroStock faz parte do meu portfólio de projetos voltados à aplicação de dados, tecnologia e automação no agronegócio.
A proposta é demonstrar como uma necessidade operacional pode ser transformada em uma solução simples, testada na prática e posteriormente evoluída utilizando ferramentas de análise de dados e automação.

👩‍💻 Projeto
AgroStock — Controle e rastreabilidade de estoque de insumos agrícolas
Projeto baseado em uma solução real utilizada em uma operação agrícola.
Status: ✅ Processo implementado e validado na operação
Próxima etapa: 🚀 Evolução para automação e análise de dados

👩‍💻 Autora:
Camyla K. Fernandes

