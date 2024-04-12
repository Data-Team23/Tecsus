# TECSUS


# Sumário
* [Introdução](#introdução)
* [Sprint 01](#sprint-01)
* [Sprint 02](#sprint-02)
* [Sprint 03](#sprint-03)
* [Sprint 04](#sprint-04)

# Introdução
Foi realizado a integração do projeto com o Sonar Cloud para a análise, revisão e correção dos problemas que podem acontecer durante o desenvolvimento do sistema.

# Sprint 01
## Problemas Encontrados
### Repositório Front-end
### :pushpin: Análises de Pull Request

__Seletor duplicado inesperado ".container"__

No CSS, quando os seletores são duplicados, o navegador os aplica em cascata. Isto significa que se dois seletores forem idênticos, o segundo terá precedência. Porém, se as declarações dentro dos seletores não forem conflitantes, elas serão combinadas.
Esse comportamento pode levar a resultados inesperados e dificultar a depuração, especialmente em folhas de estilo maiores. Portanto, geralmente é recomendado evitar a duplicação de seletores.

<p align = "center"><img width="360" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/f7cefa0c-2f77-48a6-8f78-e33f66e53f7d"></p>

O problema se encontra em: app-web/src/assets/styles/navbar.css

<p> Resolução</p>
Para corrigir seu código, remova o seletor duplicado ou mescle todas as declarações.

### Repositório Back-end
### :pushpin: Análises de Pull Request
__Refatorar função para reduzir sua complexidade cognitiva de 17 para 15 permitidas__

Complexidade Cognitiva é uma medida de quão difícil é entender o fluxo de controle de uma unidade de código. Código com alta complexidade é difícil de ler, compreender, testar e modificar.
Como regra geral, a alta complexidade cognitiva é um sinal de que o código deve ser refatorado em partes menores e mais fáceis de gerenciar.

<p align = "center"><img width="356" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/ec0d3977-c17e-4514-9bc4-f9895cae3c9e"></p>

O problema se encontra em: tecsus/contas/views.py

<p> Resolução</p>
O Sonar aponta três sugestões:

* Extraia condições complexas em uma nova função: Operadores mistos em condições aumentarão a complexidade. Extrair a condição em uma nova função com um nome apropriado reduzirá a carga cognitiva.
* Divida grandes funções: Funções grandes podem ser difíceis de entender e manter. Se uma função estiver fazendo muitas coisas, considere dividi-la em funções menores e mais gerenciáveis.
* Cada função deve ter uma única responsabilidade: Evite aninhamentos profundos retornando mais cedo.
Para evitar o aninhamento de condições, processe primeiro os casos excepcionais e retorne mais cedo.

__Remover variável não utilizada "novo_dado"__

Uma variável local não utilizada é uma variável que foi declarada, mas não é usada em nenhum lugar do bloco de código onde está definida. É um código morto, contribuindo para uma complexidade desnecessária e levando à confusão na leitura do código. Portanto, ele deve ser removido do código para manter a clareza e a eficiência.

<p align = "center"><img width="351" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/0aa5a91e-7d88-46b7-a896-5312c59d4d65"></p>

O problema se encontra em: tecsus/contas/views.py

<p> Resolução</p>

A correção para esse problema é direta. Depois de garantir que a variável não utilizada não faz parte de uma implementação incompleta que leva a bugs, basta removê-la.

__Remover atribuição à variável local 'form'; o valor nunca é usado__

Os armazenamentos mortos referem-se a atribuições feitas a variáveis ​​locais que posteriormente nunca são usadas ou são imediatamente substituídas. Tais atribuições são desnecessárias e não contribuem para a funcionalidade ou clareza do código. Eles podem até impactar negativamente o desempenho. Removê-los melhora a limpeza e a legibilidade do código. Mesmo que as operações desnecessárias não prejudiquem a correcção do programa, são - na melhor das hipóteses - um desperdício de recursos informáticos.

<p align = "center"><img width="358" alt="image" src="https://github.com/Data-Team23/Tecsus/assets/143366830/2810134c-8649-47eb-994a-eae9a0a5eda7"></p>

O problema se encontra em: tecsus/contas/views.py

<p> Resolução</p>

Remova a atribuição desnecessária e teste o código para ter certeza de que o lado direito de uma determinada atribuição não teve efeitos colaterais (por exemplo, um método que grava certos dados em um arquivo e retorna o número de bytes gravados).

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
      <td>Baixo</td>
      <td>Remover atribuição à variável local 'form'; o valor nunca é usado</td>
    </tr>
  </table>
</div>

