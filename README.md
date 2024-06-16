# TECSUS


# Sumário
* [Contexto](#contexto)
* [Equipe](#equipe)
* [Product Backlog](#product-backlog)
* [Sprint 01](#sprint-01)
* [Sprint 02](#sprint-02)
* [Sprint 03](#sprint-03)
* [Sprint 04](#sprint-04)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
  
# Contexto
[Tecsus](https://tecsus.com.br/)
A TecSUS realiza a coleta e processamento de contas de energia, água e gás para diversas empresas dos setores do atacado e varejo. Cada conta coletada precisa ter todos os seus campos digitados e salvos em banco de dados para eventuais consultas e análises técnicas/financeiras que podem trazer ao cliente oportunidades de redução de custos e alteração de contratos. 
Cada unidade do cliente pode possuir vários contratos (água, energia ou gás), cada contrato pode possuir uma ou mais contas (faturas de água, energia ou gás) por mês. Todos esses contratos estão ligados a uma concessionária de abastecimento. A Tecsus possuem uma base de dados de unidades, contratos, contas e concessionárias desestruturada em arquivo texto, a empresa tem interesse em aplicar técnicas de ETL e utilizar ferramentas de visualização de dados do mercado.

# Requisitos Funcionais
> _Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas_

> _Relatório de consumo total de água mensal, anual e média_

> _Relatório de consumo total de energia mensal, anual e média_

> _Geração de alertas de consumo acima da média (acima da média dos últimos 3 meses)_



# Equipe

> _Product Owner_ - [Alan Morato](https://www.linkedin.com/in/alan-morato-37b214154/)

> _Scrum Master_ - [Elizabeth Cristina Alves Leite](https://www.linkedin.com/in/elizabeth-cristina-alves-leite-176a9416a)

> _Dev. Team_ - [Ariane Cristina](https://www.linkedin.com/in/ariane-sousa77/)

> _Dev. Team_ - [Lucas Emanoel](https://www.linkedin.com/in/lucas-emanoel-teixeira-engracio-da-silva-ab5611234/)

> _Dev. Team_ - [Tobias Fernandes Bezerra Sousa](https://www.linkedin.com/in/tobias-sousa-23bba822a)

> _Dev. Team_ - [Julia Quitério](https://www.linkedin.com/in/j%C3%BAlia-quit%C3%A9rio-934894205/)

> _Dev. Team_ - [Murilo Junior](https://www.linkedin.com/in/murilo-jos%C3%A9-de-brito-junior-32403b157/)

> _Dev. Team_ - [Silas Prado](https://www.linkedin.com/in/silasprd/)

# Product Backlog
<div>
  <table>
    <tr>
      <td><b>Ranking</b></td>
      <td><b>Backlog</b></td>
      <td><b>Pioridade</b></td>
      <td><b>User Story</b></td>
      <td><b>Estimativa (Em dias)</b></td>
      <td><b>Sprint</b></td>
      <td><b>Requisito</b></td>
    </tr>
    <tr>
      <td>1</td>
      <td>Consumo de arquivo de dados</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de energia mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio</td>
      <td>05</td>
      <td>01</td>
      <td>Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Relatórios de Consumo Energia</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de energia mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.</td>
      <td>01</td>
      <td>01</td>
      <td>Relatório de consumo total de energia mensal, anual e média</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Relatórios de Consumo água</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de água mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.</td>
      <td>01</td>
      <td>01</td>
      <td>Relatório de consumo total de água mensal, anual e média</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Alerta de Consumo</td>
      <td>Alta</td>
      <td>Como um analista técnico/financeiro da TecSUS, Gostaria de receber alertas automatizados Para identificar consumos de água, energia ou gás que excedam a média dos últimos 3 meses De modo a poder tomar medidas proativas para investigar possíveis anomalias.</td>
      <td>05</td>
      <td>02</td>
      <td>Geração de alertas de consumo acima da média (acima da média dos últimos 3 meses)</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Cadastro de Concessionárias</td>
      <td>Média</td>
      <td>Como um funcionário da TecSUS responsável pelo gerenciamento de dados, Gostaria de cadastrar as concessionárias de abastecimento de energia, água e gás
Para garantir que as informações estejam atualizadas e disponíveis para associação com os contratos e unidades dos clientes.</td>
      <td>05</td>
      <td>03</td>
      <td>Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Cadastro de Contratos</td>
      <td>Média</td>
      <td>Como um colaborador da TecSUS encarregado do gerenciamento de contratos, Gostaria de registrar os contratos de fornecimento de energia, água e gás para cada cliente Para manter um registro organizado e preciso das obrigações contratuais e dos serviços prestados.</td>
      <td>05</td>
      <td>03</td>
      <td>Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Controle de Usuários</td>
      <td>Baixa</td>
      <td>Como um membro da equipe da TecSUS encarregado da gestão de unidades dos clientes, Gostaria de cadastrar as usuários no sistema para que seja possível liberar acessos a novos usuários da empresa.</td>
      <td>05</td>
      <td>04</td>
      <td>Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas</td>
    </tr>
  </table>
</div>


# Requisitos Sprint 01
<div>
  <table>
    <tr>
    <td><b>Backlog</b></td>
    <td><b>Importância</b></td>
  </tr>
  <tr>
   <td>Consumo de arquivo de dados</td>
   <td>Alta</td>
  </tr>
  <tr>
   <td>Relatório de consumo total de água mensal, anual e média</td>
   <td>Alta</td>
  </tr>
  <tr>
   <td>Relatório de consumo total de Energia mensal, anual e média</td>
   <td>Alta</td>
  </tr>
  </table>
</div>

# Tecnologias Utilizadas
- ``Python``
- ``JavaScript``
- ``Vue``
- ``HTML``
- ``CSS``
- ``Oracle SQL``

# Sprint 01

<img width="884" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/8df8f7ec-d3f7-4b72-b37f-57a8e4508686">

## User Stories
### Upload de Arquivos
Como gestor técnico desejo que meu sistema seja capaz de ler um arquivo de texto ou CSV e convertê-lo em uma tabela após ser carregado, para que os dados possam ser manipulados dentro do sistema

#### Critérios de aceitação
> _Necessário abrir pop up para selecionar arquivo_

> _Necessário transformar o arquivo para tabela_

> _Necessário uma barra de texto para inserir o path do arquivo_

> _Necessário selecionar Unidade, Concessionária e Contrato antes do upload_

> _Link do Figma: https://www.figma.com/file/yLpfQGjREQGfA3Ock19Awx/API-5ºSEM?type=design&node-id=1%3A2&mode=design&t=iHoVfNpxjKEGsc3H-1

### Relatório Mensal de Energia
Como Gestor Desejo um relatório com consumo total de energia mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.
#### Critérios de aceitação
> _Visibilidade mensal dos dados (Gráfico de linhas)_

> _Visibilidade de consumo total_

> _Visibilidade de gasto total_

> _Visibilidade de gasto mensal_


### Relatório Mensal de Gás
Como Gestor Desejo um relatório com consumo total de Gás mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.
#### Critérios de aceitação
> _Visibilidade mensal dos dados (Gráfico de linhas)_

> _Visibilidade de consumo total_

> _Visibilidade de gasto total_

> _Visibilidade de gasto mensal_


### Relatório Mensal de Água
Como Gestor Desejo um relatório com consumo total de água mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.
#### Critérios de aceitação
> _Visibilidade mensal dos dados (Gráfico de linhas)_

> _Visibilidade de consumo total_

> _Visibilidade de gasto total_

> _Visibilidade de gasto mensal_


--------


# Sprint 02

![image](https://github.com/Data-Team23/Tecsus/assets/102003274/fcd75cd4-d62a-40c9-b03d-575f4c9262ff)


## Requisitos Sprint 02
<div>
  <table>
    <tr>
    <td><b>Backlog</b></td>
    <td><b>Importância</b></td>
  </tr>
  <tr>
   <td>Geração de alertas de consumo acima da média (acima da média dos últimos 3 meses)</td>
   <td>Alta</td>
  </tr>
  </table>
</div>

## User Stories
### Alerta de Consumo
Como um usuário preocupado com meus gastos de energia, desejo receber alertas quando meu consumo de energia ultrapassar a média dos últimos três meses, para que eu possa identificar e corrigir comportamentos de consumo excessivo.

#### Critérios de aceitação
> _O sistema deve calcular a média do consumo de energia dos últimos três meses para o usuário.

> _Se o consumo de energia atual ultrapassar a média calculada, um alerta deve ser gerado e enviado para o usuário.

> _O alerta deve conter informações claras sobre o período de tempo em que o consumo foi alto.

> _Os alertas devem ser entregues de forma clara e compreensível por e-mail

> _O cálculo da média e a comparação com o consumo atual devem ser realizados de forma eficiente para garantir uma resposta rápida ao usuário.

> _Os alertas devem ser precisos e confiáveis, evitando falsos positivos ou negativos sempre que possível.

> _Os testes de unidade e integração devem ser implementados para garantir a funcionalidade correta do sistema, verificando o cálculo da média, a comparação com o consumo atual e a geração adequada de alertas.


### Registro de consumo acima da média
Como um administrador do sistema, desejo ter um registro de todos os alertas de consumo de energia acima da média gerados para os usuários, para que eu possa monitorar e analisar padrões de consumo em toda a base de clientes.

#### Critérios de aceitação
> _Deve haver uma tabela no banco de dados designada para armazenar os registros de alertas de consumo acima da média.

> _Identificador único do alerta.

> _Identificador do usuário para o qual o alerta foi gerado.

> _Consumo atual que acionou o alerta.

> _Média do consumo de energia dos últimos três meses para o usuário.

> _O sistema deve registrar automaticamente os alertas sempre que forem gerados para os usuários.



### Cálculo da Média
Como um sistema de gerenciamento de energia, desejo ter um método eficiente para calcular a média do consumo de energia dos últimos três meses para um usuário específico, para que eu possa identificar quando o consumo atual excede essa média e gerar alertas apropriados.
#### Critérios de aceitação
> _O sistema deve ser capaz de calcular a média do consumo de energia dos últimos três meses para um usuário específico.

> _O cálculo da média deve levar em consideração apenas os dados de consumo dos últimos três meses disponíveis para o usuário.

> _A média calculada deve ser precisa e refletir com precisão o padrão de consumo do usuário ao longo do tempo.

> _O sistema deve ser capaz de lidar com diferentes unidades de medida  e converter adequadamente os valores, se necessário, para calcular a média.



### Tratamento de Dados
Como um sistema de gerenciamento de energia, desejo ter um mecanismo robusto para comparar o consumo de energia atual de um usuário com a média dos últimos três meses e gerar alertas quando o consumo atual excede essa média, para ajudar os usuários a identificar e corrigir padrões de consumo excessivo.
#### Critérios de aceitação
> _Tratar dados nulos de todas as colunas

> _Tratar dados duplicados das colunas

> _Tratar dados inválidos das colunas


### Conexão com e-mail
Como um usuário preocupado com meus gastos de energia, desejo receber alertas por email quando meu consumo de energia ultrapassar a média dos últimos três meses, para que eu possa identificar e corrigir comportamentos de consumo excessivo de forma rápida e eficiente.
#### Critérios de aceitação
> _O sistema deve ter integração com o gmail.

> _O sistema precisa ter uma mensagem preparada para ser enviada

### Versionamento do Power BI
Como um usuário da TecSUS eu gostaria de o power BI versionado no github, para que eu possa a versão mais atualizada do board.
#### Critérios de aceitação
> _Melhorar visualizações do dashboard e trazer mais informações relevantes para o negócio

> _Realizar o versionamento do BI dentro do github

> _Documentar cada visualização

_Exemplo> Vídeo de consulta: https://www.youtube.com/watch?v=rTbSsVFeeI0_



--------

# Sprint 03


![image](https://github.com/Data-Team23/Tecsus/assets/102003274/50044d76-455f-47ec-94cb-492818271d4d)


## Requisitos Sprint 03
<div>
  <table>
    <tr>
    <td><b>Backlog</b></td>
    <td><b>Importância</b></td>
  </tr>
  <tr>
   <td>> Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas</td>
   <td>Alta</td>
  </tr>
  </table>
</div>

## User Stories
### Cadastro de Fornecedor/Unidade
Como um funcionário da TecSUS responsável pelo gerenciamento de dados, Gostaria de cadastrar os fornecedores e Unidades de abastecimento de água e energia. Para garantir que as informações estejam atualizadas e disponíveis para associação com os contratos e unidades dos clientes.

#### Critérios de aceitação
> _O sistema deve permitir o cadastro de novos fornecedores, incluindo informações relevantes para a identificação do mesmo_

> _Deve ser possível editar e atualizar as informações dos fornecedores existentes_

> _As informações cadastradas de fornecedores e unidades de abastecimento devem estar sempre atualizadas e disponíveis para consulta_

> _Deve ser possível associar os fornecedores e unidades de abastecimento aos contratos dos clientes, garantindo uma gestão integrada_

### Cadastro de Clientes/Contratos
Como um colaborador da TecSUS encarregado do gerenciamento de contratos, Gostaria de registrar os clientes/contratos de fornecimento de água e energia para cada cliente Para manter um registro organizado e preciso das obrigações contratuais e dos serviços prestados

#### Critérios de aceitação
> _O sistema deve permitir o cadastro de novos clientes, incluindo informações relevantes para a identificação

> _Deve ser possível associar um ou mais contratos de fornecimento de água e energia a cada cliente_

> _Deve ser possível editar e atualizar as informações dos fornecedores existentes_

> _Deve ser possível associar os fornecedores e unidades de abastecimento aos contratos dos clientes, garantindo uma gestão integrada_


### Modelagem tipo Estrela
Como um usuário da TecSUS eu gostaria de ter um banco de dados em estrela para armazenar os dados de unidades, concessionárias, contratos e contas, para que eu possa realizar análises técnicas e financeiras de forma eficiente e gerar relatórios de consumo de água, energia e gás.
> _Como administrador do sistema, quero poder extrair os dados de unidades, concessionárias, contratos e contas de arquivos de texto desestruturados para carregá-los no banco de dados em estrela.

> _Como usuário, desejo que os dados no banco de dados em estrela sejam transformados de maneira consistente e padronizada, garantindo a integridade e a qualidade das informações.

> _Como usuário, quero que o banco de dados em estrela seja projetado de forma a permitir consultas eficientes para a geração de relatórios de consumo de água, energia e gás mensais, anuais e médios.

> _Como usuário, desejo que o banco de dados em estrela inclua um mecanismo de geração de alertas para identificar consumos acima da média nos últimos 3 meses.

> _Como parte dos requisitos não funcionais, desejo que seja implementada uma esteira de DevOps para garantir a integração contínua, entrega contínua e automação de processos de desenvolvimento, teste e implantação da solução proposta.


# Sprint 04
![WhatsApp Image 2024-06-16 at 15 56 28](https://github.com/Data-Team23/Tecsus/assets/108765052/4fbd3950-3574-4f7a-a384-23476000f849)

## Requisitos Sprint 03
<div>
  <table>
    <tr>
    <td><b>Backlog</b></td>
    <td><b>Importância</b></td>
  </tr>
  <tr>
   <td>> Extrair, Transformar e Carregar os dados de Unidades, Concessionárias, Contratos e Contas</td>
   <td>Alta</td>
  </tr>
  </table>
</div>

### Validação e Implementação do Teste de Qualidade de Software
Como usuário do sistema, eu quero que a qualidade do software seja aprimorada para que eu possa ter uma experiência mais confiável e satisfatória ao utilizar o sistema.

> _ Todas as funcionalidades do sistema devem ser testadas para garantir que funcionem conforme o esperado.

> _Os testes automatizados devem ser implementados para garantir a detecção precoce de possíveis regressões.

> _A equipe de desenvolvimento deve realizar revisões de código regularmente para garantir a qualidade do código-fonte.

> _Métricas de qualidade, como cobertura de código e taxa de defeitos, devem ser monitoradas e melhoradas ao longo do tempo.

> _O feedback dos usuários deve ser coletado e utilizado para identificar áreas de melhoria contínua na qualidade do software.



### Implementação do Processo de Deploy Automatizado
Como administrador do sistema, quero que o processo de deploy seja automatizado e confiável, para que as novas versões do software possam ser implantadas de maneira eficiente e sem erros.

> _O processo de deploy deve ser totalmente automatizado, desde a integração contínua até a entrega contínua.

> _O deploy deve garantir a estabilidade do sistema.

> _O pipeline de deploy deve passar por uma série de testes automatizados para garantir que a nova versão do software esteja livre de erros.


### Deploy do Banco
Como administrador do sistema, quero que o processo de deploy do banco de dados seja automatizado e confiável, para que as atualizações de schema e dados possam ser implantadas de maneira eficiente e sem erros.

> _Criação de versionamento pra banco de dados

> _Criação de cargas para regras de banco

> _Testes para carga

### Criação e Manutenção da Documentação do Projeto
Como membro da equipe de desenvolvimento, quero ter uma documentação clara e atualizada do projeto para que todos possam compreender facilmente o propósito, funcionamento e arquitetura do sistema, facilitando a manutenção, comunicação externa e aprendizado contínuo.

> _A documentação deve fornecer uma explicação clara do propósito, funcionamento e arquitetura do projeto.

> _A documentação deve ser mantida detalhada e atualizada para facilitar a manutenção e as atualizações do código.

> _A documentação deve estar disponível para comunicação externa com partes interessadas, como clientes ou parceiros.

> _O Wiki do GitHub deve ser utilizado como a ferramenta principal para a criação e manutenção da documentação.


### Implementação dos Testes de Integração
Como desenvolvedor, quero implementar testes de integração para verificar todas as funcionalidades implementadas na branch Developer, possibilitando a identificação precoce de problemas e garantindo a qualidade do software antes do deploy.

> _Os testes de integração devem verificar todas as funcionalidades implementadas na branch Developer.

> _Os testes de integração devem ser capazes de identificar possíveis problemas que possam surgir ao juntar as funcionalidades.

> _Um ambiente de testes deve ser criado no GitHub.

> _Os gatilhos para acionar os testes de integração devem ser definidos (e.g., push na branch Developer, pull request, merge).


### Controle de Usuários

Como membro da equipe da TecSUS encarregado da gestão de unidades dos clientes, gostaria de cadastrar usuários no sistema para que seja possível liberar acessos a novos usuários da empresa.

> _Deve ser possível cadastrar novos usuários no sistema com as informações necessárias (nome, e-mail, cargo, etc.).

> _Os novos usuários devem receber um e-mail de confirmação e instruções para ativar suas contas.

> _Os dados dos novos usuários devem ser validados antes de serem salvos no sistema.

> _Deve haver uma interface amigável e intuitiva para o cadastro de novos usuários.
