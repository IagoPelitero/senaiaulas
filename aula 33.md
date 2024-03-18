Aula 33 correção do desafio.

código do professor inicialmente usado:

~~~js

const nota1 = 10;
const nota2 = 6;
const nota3 = 7;

const soma = nota1 + nota2 + nota3;
const media = soma/3;

const condicaoAprovado = media >= 7;
const condicaoExame = media < 7 && media >= 5;

if (condicaoAprovado){
    console.log(`O aluno está Aprovado com média ${media}`);
} else if (condicaoExame) {
    console.log(`O aluno está em Exame com média ${media}`);
} else {
    console.log(`O aluno está Reprovado com media ${media}`);
}

~~~

Mudanças no código:

~~~js
const 
    nota1 = 3,
    nota2 = 0,
    nota3 = 7,
    media = (nota1 + nota2 + nota3) / 3;

if (media >= 7){
    console.log(`O aluno está Aprovado com média ${media.toFixed(2)}`);
} else if (media >= 5){
    console.log(`O aluno está em Exame com média ${media.toFixed(2)}`);
} else {
    console.log(`O aluno está Reprovado com media ${media.toFixed(2)}`);
}
~~~

O JavaScript já transforma em objeto as varáveis.

Quando acrescentamos `.toFixed(quantidade de prefixos mostrados)` ele limita os números mostrados ao usuário.
