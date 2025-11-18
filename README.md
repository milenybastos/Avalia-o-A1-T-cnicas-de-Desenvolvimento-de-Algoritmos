# A1TDA_SI
#  Estruturas Condicionais - Sistemas de Informação (2º Semestre)

## 1. Sistema de Verificação de Idade

### Descrição
Um programa interativo que simula o controle de entrada de uma balada. O objetivo foi praticar o uso de **Guard Clauses** (verificação antecipada de erros) para tornar o código mais limpo, evitando o aninhamento excessivo de `if/else`.

**Conceitos aplicados:**
* Estruturas condicionais (`if`, `elif`, `else`).
* Tratamento de erros com `try` e `except` (para evitar que letras quebrem o programa).
* Entrada e saída de dados (`input`, `print`, `f-strings`).

###  Exemplos de Entrada e Saída
==============================================
     Sistema de Entrada 
==============================================
Qual a sua idade? 20

[APROVADO] 
Idade: 20. Acesso total. Pode pegar a pulseira VIP.

==============================================

==============================================
     Sistema de Entrada    
==============================================
Qual a sua idade? 17

[APROVADO COM RESTRIÇÃO] 
Idade: 17. Acesso à pista, mas longe do bar. Pulseira Jovem.

==============================================

==============================================
     Sistema de Entrada    
==============================================
Qual a sua idade? 14

[BARRADO] 
Idade: 14. Desculpe, festa só para maiores de 16.

==============================================

==============================================
     Sistema de Entrada    
==============================================
Qual a sua idade? vinte

[ERRO DE ENTRADA] 
O que você digitou ('vinte') não é um NÚMERO.
Rode o programa de novo e digite sua idade com números.

==============================================

==============================================
     Sistema de Entrada   
==============================================
Qual a sua idade? -5

[IDADE INEXISTENTE] 
Idade '-5'? Isso não é válido. Tente de novo.

==============================================

---

## 2. Contador de Números Pares (Laços For/While)

###  Descrição
Exercício para praticar estruturas de repetição. O programa implementa duas versões de um contador que exibe todos os números pares entre 1 e 100.

**Conceitos aplicados:**
* Laço de repetição `for` com `range()`.
* Laço de repetição `while` com controle manual de contador.
* Operador lógico (módulo `%`) para verificar se um número é par.

### Exemplo de Uso:

==============================================
     Contador de Pares com 'for' e 'while'    
==============================================

--- Números Pares (usando FOR) ---
2
4
6
( ... )
98
100

--- Números Pares (usando WHILE) ---
2
4
6
( ... )
98
100

==============================================
Fim da contagem!

---

## 3. Cadastro de Alunos (Listas)

###  Descrição
Programa que demonstra o uso de listas para armazenar dados de forma dinâmica. O usuário pode inserir quantos nomes de alunos desejar. O programa utiliza um laço `while True` para a entrada contínua e uma condição de parada (a palavra 'fim') para encerrar a coleta de dados.

**Conceitos aplicados:**
* **Listas**: Criação de uma lista vazia `[]`.
* **Método `.append()`**: Para adicionar novos itens ao final da lista.
* **Laço `while True` com `break`**: A forma mais comum de criar um loop que espera uma entrada específica do usuário.
* **Laço `for`**: Para iterar (percorrer) a lista e exibir cada item.
* **Função `len()`**: Para contar o número de itens na lista.

==============================================
     Cadastro de Alunos (usando Listas)     
==============================================
Digite os nomes dos alunos. Digite 'fim' para parar.
Digite o nome do aluno: Ana
'Ana' adicionado. (Total: 1)
Digite o nome do aluno: Bruno
'Bruno' adicionado. (Total: 2)
Digite o nome do aluno: Carla
'Carla' adicionado. (Total: 3)
Digite o nome do aluno: fim

==============================================
--- Lista Final de Alunos Cadastrados (3) ---
- Pedro
- João Miguel
- Mariana
- Mileny

==============================================
---

## 4. Cadastro de Produtos (Dicionários)

###  Descrição
Sistema simples para cadastrar produtos (nome) e seus respectivos preços (valor). Este exercício demonstra o uso de **dicionários** (`dict`) para criar um mapeamento chave-valor.

**Conceitos aplicados:**
* **Dicionários**: Criação de um dicionário vazio `{}`.
* **Inserção de Dados**: `dicionario[chave] = valor`.
* **Tratamento de Erros**: Uso de `try...except ValueError` para garantir que o preço seja um número.
* **Verificação de Chave**: Uso do `in` para checar se um produto já existe.
* **Iteração com `.items()`**: Para percorrer o dicionário e obter tanto a chave (nome) quanto o valor (preço).
* **Formatação de Strings**: Uso de `f-strings` com `:.2f` para formatar o preço.

==============================================
     Cadastro de Produtos (usando Dict)     
=============================================="
Digite 'fim' no nome do produto para parar.

Digite o nome do produto: Teclado
Digite o preço para 'Teclado': R$ 150.90
Produto 'Teclado' - R$ 150.90 cadastrado!

Digite o nome do produto: Mouse
Digite o preço para 'Mouse': R$ 80
Produto 'Mouse' - R$ 80.00 cadastrado!

Digite o nome do produto: Monitor
Digite o preço para 'Monitor': R$ abc
Erro: O preço deve ser um número (ex: 10.50). Produto não cadastrado.

Digite o nome do produto: Monitor
Digite o preço para 'Monitor': R$ 700.00
Produto 'Monitor' - R$ 700.00 cadastrado!

Digite o nome do produto: fim

==============================================
--- Lista Final de Produtos (3) ---
Produto: Teclado | Preço: R$ 150.90
Produto: Mouse | Preço: R$ 80.00
Produto: Monitor | Preço: R$ 700.00
==============================================
