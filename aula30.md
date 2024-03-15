# Escopo

Exemplo: Quando temos uma instrução como arrumar a cadeira embaixo da cadeira na sala de aula é uma instrução local, ou seja, vale apenas na sala de aula.

A global vale para qualquer ambiente como jogar o lixo no lixo.

O root tem propriedade de escopo global.

*Nomeando varáveis (definindo o seu iedntificador):*
*kebab-case -> Ex:"minha-variavel-numerica"
under_case ou snake_case -> Ex:"minha_variavel_numeria"
camelCase -> Ex:"minhaVariavelNumerica"
PascalCase -> Ex:"MinhaVariavelNumerica"*

let minhaVariavel = 'iago'; (quando possui ' -> aspas simples é texto)

'string' -> texto
'number' -> número


Aula sobre tipagem:
let minhaVariavel = 'iago';

~~~js
`undefined
ty
VM176:1 Uncaught ReferenceError: ty is not defined
    at <anonymous>:1:1
(anonymous) @ VM176:1
typeof(minhaVariavel)
'string'
minhaVariavel = 38;
38
typeof(minhaVariavel)
'number'
minhaVariavel = 1.79
1.79
typeof(minhaVariavel)
'number'
minhaVariavel = 1.739821648732657361498643785687368916298618753872
1.7398216487326574
typeof(minhaVariavel)
'number'
minhaVariavel = 'a'
'a'
typeof(minhaVariavel)
'string'
minhaVariavel = asftd4343462
VM591:1 Uncaught ReferenceError: asftd4343462 is not defined
    at <anonymous>:1:1
(anonymous) @ VM591:1
minhaVariavel = true
true
typeof(minhaVariavel)
'boolean'
minhaVariavel = {id: 1, nome: 'iago'}
{id: 1, nome: 'iago'}
typeof(minhaVariavel)
'object'
console.log(minhaVariavel.id);
VM926:1 1
undefined
console.log(minhaVariavel.nome);
VM952:1 iago
undefined
minhaVariavel = {id: 1, nome: 'iago', instrutor: true}
{id: 1, nome: 'iago', instrutor: true}
console.log(minhaVariavel.instrutor);
VM1027:1 true
undefined
minhaVariavel = [1, 2, 3, 4, 5];
(5) [1, 2, 3, 4, 5]
typeof(minhaVariavel)
'object'
minhaVariavel []
VM1106:1 Uncaught SyntaxError: Unexpected token ']'
minhaVariavel [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
undefined
minhaVariavel = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
(3) [Array(3), Array(3), Array(3)]
typeof(minhaVariavel)
'object'`
~~~

# Operadores de atribuição:
= -> valor atribuido à variável
+= -> atribui somando o novo valor
-= -> atribui subtraindo o novo valor
*= -> atribui multiplicando o novo valor
/= -> atribui dividindo o novo valor

# Operadores aritméticos:
+ -> soma
- -> subtração
* -> multiplicação
/ -> divisão
% -> resto da divisão (módulo)

# operadores de incremento e decremento:
++ -> incremento (soma 1)
-- -> decremento (subtra 1)


Obs: quando for incluir o código após ctrl + l cuidado para não atualizar em F5 (quando atualiza precisa reatribuir com 'let')

Na leitura do JavaScript primeiro lê-se linha a linha.

Exemplo: 
vairavel ++ (pós-incremento)
++ variavel (pré-incremento)
variavel -- (pós-decremento)
-- variavel (pós-incremento)
