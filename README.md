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

> _Relatório de consumo total de gás mensal, anual e média_

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
    </tr>
    <tr>
      <td>1</td>
      <td>Consumo de arquivo de dados</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de energia mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio</td>
      <td>05</td>
      <td>01</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Relatórios de Consumo Energia</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de energia mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.</td>
      <td>01</td>
      <td>01</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Relatórios de Consumo Gás</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de Gás mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.</td>
      <td>01</td>
      <td>01</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Relatórios de Consumo água</td>
      <td>Alta</td>
      <td>Como Gestor Desejo um relatório com consumo total de água mensal, anual e média Para que seja possível analisar as tendências e ter acesso a métricas importantes para o negócio.</td>
      <td>01</td>
      <td>01</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Alerta de Consumo</td>
      <td>Alta</td>
      <td>Como um analista técnico/financeiro da TecSUS, Gostaria de receber alertas automatizados Para identificar consumos de água, energia ou gás que excedam a média dos últimos 3 meses De modo a poder tomar medidas proativas para investigar possíveis anomalias.</td>
      <td>05</td>
      <td>02</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Cadastro de Concessionárias</td>
      <td>Média</td>
      <td>Como um funcionário da TecSUS responsável pelo gerenciamento de dados, Gostaria de cadastrar as concessionárias de abastecimento de energia, água e gás
Para garantir que as informações estejam atualizadas e disponíveis para associação com os contratos e unidades dos clientes.</td>
      <td>05</td>
      <td>03</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Cadastro de Contratos</td>
      <td>Média</td>
      <td>Como um colaborador da TecSUS encarregado do gerenciamento de contratos, Gostaria de registrar os contratos de fornecimento de energia, água e gás para cada cliente Para manter um registro organizado e preciso das obrigações contratuais e dos serviços prestados.</td>
      <td>05</td>
      <td>03</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Cadastro de Unidades</td>
      <td>Média</td>
      <td>Como um membro da equipe da TecSUS encarregado da gestão de unidades dos clientes, Gostaria de cadastrar as unidades dos clientes, identificando-as por localização e características específicas Para organizar os dados e facilitar a associação com os contratos e as contas de consumo de energia, água e gás.</td>
      <td>05</td>
      <td>03</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Controle de Usuários</td>
      <td>Baixa</td>
      <td>Como um membro da equipe da TecSUS encarregado da gestão de unidades dos clientes, Gostaria de cadastrar as unidades dos clientes, identificando-as por localização e características específicas Para organizar os dados e facilitar a associação com os contratos e as contas de consumo de energia, água e gás.</td>
      <td>05</td>
      <td>04</td>
    </tr>
  </table>
</div>


# Backlog Sprint 01
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
   <td>Relatórios de Consumo</td>
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
> _O sistema deve enviar automaticamente um email ao usuário sempre que seu consumo de energia ultrapassar a média dos últimos três meses.

> _O email de alerta deve conter informações claras sobre o período de tempo em que o consumo foi alto, incluindo datas e valores de consumo.

> _O sistema deve permitir alguma forma de personalização do conteúdo do email, como o uso do nome do usuário e a possibilidade de adicionar ou remover informações específicas de acordo com as preferências do usuário.

> _Teste de Envio de Email: Os testes de integração devem ser implementados para garantir que os emails de alerta sejam enviados corretamente sempre que o consumo de energia ultrapassar a média, verificando se o conteúdo está completo e se o email é entregue ao endereço correto.








