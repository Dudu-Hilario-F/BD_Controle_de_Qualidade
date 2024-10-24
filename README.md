# Projeto de Banco de Dados para gerenciamento de um centro de distribuição alimentícios
***Por mais que os problemas citados aqui sejam reais, esse projeto é para fins acadêmicos e testes***  

## Índices

 1. Arquitetura
 2. Quais problemas o projeto resolve
 3. Aplicativos usados
 4. Como se conectar ao banco de dados
    
# Arquitetura
Esse projeto nasceu da necessidade de resolver um problema enfrentado no centro de distribuição de alimentos perecíveis, especificamente no setor de qualidade. O profissional da qualidade tem a função de receber, analisar e aprovar os produtos, além de acompanhar o armazenamento adequadamente dessas mercadorias, monitorar o produto, manter controle de validade e realizar o PEPS (Primeiro a Entrar, Primeiro a Sair). Oprofissional é também responsável por identificar problemas a partir das reclamações das filiais e monitorar as temperaturas dos alimentos e do ambiente.

Entretanto, esse profissional enfrenta desafios significativos devido à falta de acesso ao sistema da empresa e à ausência de um computador para acompanhar esses alimentos desde o recebimento até a expedição. Essa situação dificultava a realização das tarefas desse profissional, gerando retrabalho e aumentando a possibilidade de erros.

### Quais problemas esse projeto resolve:
Esse projeto resolve diversos problemas, mas os principais são:

* 1 - O profissional poderá ter controle do CD desde o recebimento da mercadoria até sua expedição
* 2 - O profissional terá controle sobre o armazenamento dessas mercadorias
* 3 - Vai permitir acompanha a temperatura da camara fria diariamente e o impacto sobre os alimentos
* 4 - O profissional poderá saber quais foram as variações dos alimentos dentro da camara

### Aplicativos usados
* Lucidchart para modelagem de dados: (https://www.lucidchart.com/pages/pt)
## 2. Como se conectar ao banco de dados
***A versão do banco de dados usado para teste foi: oracle 19c Autonomos Database***

você pode usar ferramentas como SQL Developer, SQLcl, ou até mesmo o JDBC para conectar-se ao banco, mas nesse tutorial vou ensinar apenas dois.

### Exemplo 1: Usando o SQL Develope
Passo a Passo:

* Baixe os arquivos desse repositorio
* Extrai o arquivo do repositorio e vá na pasta **Arquivos**
* Abra a pasta sqldeveloper e executa o **sqldeveloper.exe** dentro da pasta
* Com o sqldeveloper aberto vá para **New Connection (Nova Conexão) clicando no ícone de "+" no canto superior esquerdo**.
* Na tela aberta preencha os detalhes da conexão:
  * Connection Name **(Nome)**: Nome da sua conexão, pode ser qualquer nome.
  * Username (usuario): Digite **Oracle_teste** seu usuario teste.
  * Password (senha): A senha definida ao criar o banco.
  * Connection Type **(Tipo de Conexão)**: Selecione Cloud Wallet.
  * Configuration File **(Arquivo de configuração)**: Navegue até o diretório onde você baixou o arquivo desse diretorio vá na pasta wallet e selecione **Wallet** em zip.
  * Service Name **(Serviços)**: Selecione o serviço correspondente (exemplo: dbname_high ou dbname_low).
  * Testar e Conectar: Clique em Test para testar a conexão.
  * Se estiver tudo correto, clique em Connect para se conectar ao banco de dados.

