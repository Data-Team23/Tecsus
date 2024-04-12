# TECSUS


# Sumário
* [Introdução](#introdução)
* [Sprint 01](#sprint-01)
* [Sprint 02](#sprint-02)
* [Sprint 03](#sprint-03)
* [Sprint 04](#sprint-04)

# Introdução
Foi realizado a integração do projeto com o Sonar Cloud para a análise, revisão e manutenção dos problemas que podem acontecer durante o desenvolvimento do sistema.

Link do Sonar Cloud - Front-end: https://sonarcloud.io/project/overview?id=Data-Team23_Tecsus-frontend

Link do Sonar Cloud- Back-end: https://sonarcloud.io/project/overview?id=Data-Team23_Tecsus-backend

# Sprint 01
## Problemas Encontrados
### Repositório Front-end
### :pushpin: Análises de Pull Request

__Seletor duplicado inesperado ".container"__

<p>No CSS, quando os seletores são duplicados, o navegador os aplica em cascata. Isto significa que se dois seletores forem idênticos, o segundo terá precedência. Porém, se as declarações dentro dos seletores não forem conflitantes, elas serão combinadas.
Esse comportamento pode levar a resultados inesperados e dificultar a depuração, especialmente em folhas de estilo maiores. Portanto, geralmente é recomendado evitar a duplicação de seletores.</p>

<p align = "center"><img width="360" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/f7cefa0c-2f77-48a6-8f78-e33f66e53f7d"></p>

<p>O problema se encontra em: app-web/src/assets/styles/navbar.css</p>

__Resolução__
<p>Para corrigir seu código, remova o seletor duplicado ou mescle todas as declarações.</p>
<br><br>

__Seletor de pseudoelemento desconhecido inesperado "::file-selector-text"__

<p>As especificações W3C definem os seletores de pseudoelementos válidos. Somente os seletores de pseudoelementos oficiais e específicos do navegador devem ser usados ​​para obter o impacto esperado na renderização final.</p>

<p align = "center"><img width="356" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/73217b22-70a7-49d4-8553-2208deee45a6"></p>

<p>O problema se encontra em: app-web/src/components/InputField/styles.css</p>

__Resolução__
<p>É necessário utilizar somente os seletores de pseudoelementos oficionais e específicos do navegador.</p>
<br><br>

__Adicionar uma descrição a tabela - Table.vue__

<p>Para serem acessíveis aos usuários com deficiência visual, é importante que as tabelas forneçam uma descrição do seu conteúdo antes dos dados serem acessados.</p>

<p align = "center"><img width="354" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/008b8ec4-4d9f-45be-8872-01d46971b14b"></p>

<p>O problema se econtra em: app-web/src/components/Table/Table.vue</p>

__Resolução__
<p>É necessário que a tabela forneça uma descrição do conteúdo antes dos dados serem acessados.</p>
<br><br>

__Remover importação não utilizada de 'ref'.__
<p>As importações desnecessárias referem-se à importação de módulos, bibliotecas ou dependências que não são usados ​​ou referenciados em nenhum lugar do código. Essas importações não contribuem para a funcionalidade do aplicativo e apenas adicionam peso extra ao pacote JavaScript, levando a possíveis problemas de desempenho e capacidade de manutenção.</p>

<p align = "center"><img width="357" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/81ed874e-f8d9-463f-8ded-75d72db8bbce"></p>

<p>O problema se encontra em: app-web/src/components/Table/Table.vue</p>

__Resolução__
<p>Para mitigar os problemas associados a importações desnecessárias, é necessário revisar e remover regularmente quaisquer importações que não estejam sendo utilizadas.</p>
<br><br>

__Adicionar cabeçalhos, tag _th_, a tag _tabela___
<p>Os cabeçalhos das tabelas são essenciais para melhorar a acessibilidade dos dados de uma tabela, especialmente para tecnologias assistivas como leitores de tela. Esses cabeçalhos fornecem o contexto necessário para transformar dados em informações. Sem cabeçalhos, os usuários se perdem rapidamente no fluxo de dados.</p>

<p align = "center"><img width="353" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/f4817b23-2d99-40bd-9e29-ef1f4fe7d8e8"></p>

<p>O problema se encontra em: app-web/src/views/Upload.vue</p>

__Resolução__
<p>A primeira tag tr da tabela deve conter elementos  da tag th, com a descrição apropriada do que os dados nas colunas representam</p>
<br><br>

__Adicionar uma descrição a tabela - Upload.vue__
<p>Para serem acessíveis aos usuários com deficiência visual, é importante que as tabelas forneçam uma descrição do seu conteúdo antes dos dados serem acessados.</p>

<p align = "center"><img width="357" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/fd497c20-0684-415a-a8d5-c3a42f6c0ec2"></p>

<p>O problema se encontra em: app-web/src/views/Upload.vue</p>

__Resolução__
<p>É necessário que a tabela forneça uma descrição do conteúdo antes dos dados serem acessados.</p>
<br><br>

### Repositório Back-end
### :pushpin: Análises de Pull Request
__Refatorar função para reduzir sua complexidade cognitiva de 17 para 15 permitidas__

<p>Complexidade Cognitiva é uma medida de quão difícil é entender o fluxo de controle de uma unidade de código. Código com alta complexidade é difícil de ler, compreender, testar e modificar.
Como regra geral, a alta complexidade cognitiva é um sinal de que o código deve ser refatorado em partes menores e mais fáceis de gerenciar.</p>

<p align = "center"><img width="356" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/ec0d3977-c17e-4514-9bc4-f9895cae3c9e"></p>

<p>O problema se encontra em: tecsus/contas/views.py</p>

<p> Resolução</p>
<p>O Sonar aponta três sugestões:</p>

* Extraia condições complexas em uma nova função: Operadores mistos em condições aumentarão a complexidade. Extrair a condição em uma nova função com um nome apropriado reduzirá a carga cognitiva.
* Divida grandes funções: Funções grandes podem ser difíceis de entender e manter. Se uma função estiver fazendo muitas coisas, considere dividi-la em funções menores e mais gerenciáveis.
* Cada função deve ter uma única responsabilidade: Evite aninhamentos profundos retornando mais cedo.
Para evitar o aninhamento de condições, processe primeiro os casos excepcionais e retorne mais cedo.
<br><br>

__Remover variável não utilizada "novo_dado"__

<p>Uma variável local não utilizada é uma variável que foi declarada, mas não é usada em nenhum lugar do bloco de código onde está definida. É um código morto, contribuindo para uma complexidade desnecessária e levando à confusão na leitura do código. Portanto, ele deve ser removido do código para manter a clareza e a eficiência.</p>

<p align = "center"><img width="351" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/0aa5a91e-7d88-46b7-a896-5312c59d4d65"></p>

<p>O problema se encontra em: tecsus/contas/views.py</p>

<p> Resolução</p>

<p>A correção para esse problema é direta. Depois de garantir que a variável não utilizada não faz parte de uma implementação incompleta que leva a bugs, basta removê-la.</p>
<br><br>

__Remover atribuição à variável local 'form'; o valor nunca é usado__

<p>Os armazenamentos mortos referem-se a atribuições feitas a variáveis ​​locais que posteriormente nunca são usadas ou são imediatamente substituídas. Tais atribuições são desnecessárias e não contribuem para a funcionalidade ou clareza do código. Eles podem até impactar negativamente o desempenho. Removê-los melhora a limpeza e a legibilidade do código. Mesmo que as operações desnecessárias não prejudiquem a correcção do programa, são - na melhor das hipóteses - um desperdício de recursos informáticos.</p>

<p align = "center"><img width="358" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/2810134c-8649-47eb-994a-eae9a0a5eda7"></p>

<p>O problema se encontra em: tecsus/contas/views.py</p>

<p> Resolução</p>

<p>Remova a atribuição desnecessária e teste o código para ter certeza de que o lado direito de uma determinada atribuição não teve efeitos colaterais (por exemplo, um método que grava certos dados em um arquivo e retorna o número de bytes gravados).</p>
<br><br>

## Priorização para correção

<div>
  <table>
    <tr>
      <td><b>Ranking</b></td>
      <td><b>Pioridade</b></td>
      <td>Problema</b></td>
    </tr>
    <tr>
      <td>1</td>
      <td>Crítico</td>
      <td>Refatorar função para reduzir sua complexidade cognitiva de 17 para 15 permitidas</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Médio</td>
      <td>Remover variável não utilizada "novo_dado"</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Médio</td>
      <td>Seletor duplicado inesperado ".container"</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Médio</td>
      <td>Adicionar cabeçalhos, tag _th_, a tag _tabela_</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Médio</td>
      <td>Seletor de pseudoelemento desconhecido inesperado "::file-selector-text"</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Baixo</td>
      <td>Remover atribuição à variável local 'form'; o valor nunca é usado</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Baixo</td>
      <td>Remover importação não utilizada de 'ref'</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Baixo</td>
      <td>Adicionar uma descrição a tabela - Table.vue</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Baixo</td>
      <td>Adicionar uma descrição a tabela - Upload.vue</td>
    </tr>
  </table>
</div>

