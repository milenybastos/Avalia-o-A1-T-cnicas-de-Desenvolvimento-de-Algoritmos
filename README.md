A1TDA_SI

Estruturas Condicionais - Sistemas de Informação (2º Semestre)

1. Sistema de Verificação de Idade

 Descrição

Um programa interativo que simula o controle de entrada de uma balada. O objetivo foi praticar o uso de Guard Clauses (verificação antecipada de erros) para tornar o código mais limpo, evitando o aninhamento excessivo de if/else.

Conceitos aplicados:

Estruturas condicionais (if, elif, else).

Tratamento de erros com try e except (para evitar que letras quebrem o programa).

Entrada e saída de dados (input, print, f-strings).


 Exemplos de Entrada e Saída

==============================================
Sistema de Entrada

Qual a sua idade? 20

[APROVADO] 
Idade: 20. Acesso total. Pode pegar a pulseira VIP.

==============================================

==============================================
Sistema de Entrada

Qual a sua idade? 17

[APROVADO COM RESTRIÇÃO] 
Idade: 17. Acesso à pista, mas longe do bar. Pulseira Jovem.

==============================================

==============================================
Sistema de Entrada

Qual a sua idade? 14

[BARRADO] 
Idade: 14. Desculpe, festa só para maiores de 16.

==============================================

==============================================
Sistema de Entrada

Qual a sua idade? vinte

[ERRO DE ENTRADA] 
O que você digitou ('vinte') não é um NÚMERO.
Rode o programa de novo e digite sua idade com números.

==============================================

==============================================
Sistema de Entrada

Qual a sua idade? -5

[IDADE INEXISTENTE] 
Idade '-5'? Isso não é válido. Tente de novo.

==============================================
