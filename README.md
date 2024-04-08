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
### :pushpin: Branch XP-22-DOCKER
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
