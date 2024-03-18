# Aula 33 correção do desafio.

código do professor inicialmente usado:

## desafio1.js

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

## desafio2.js

~~~js

const =
    altura = 1.73
    peso = 83
    imc = peso / altura ** 2;

if (imc < 1.85){
    console.log(`IMC: ${imc} -- Abaixo do peso`);
} if (imc > 18.5 && imc < 24.9){
    console.log(`IMC: ${imc} -- Peso normal`)
} if (imc > 25.o && imc < 29.9) {
    console.log(`IMC: ${imc} -- Sobrepeso`)
} if (imc > 30.o && imc < 34.9)
console.log(`IMC: ${imc} -- Obesidade grau I`)
} if (imc > 35.o && imc < 39.9)
console.log(`IMC: ${imc} -- Obesidade grau II`)
} else {
console.log(`IMC: ${imc} -- Obesidade III`)
}

~~~

Prescia ter `else-if` pois ele irá testar todos separadamente ao invés de tratar o código unicamente.

Quando trabalhamos com faixas, precisamos de intervalos abertos e fechados.

Teste 2:

~~~js
const =
    altura = 1.73
    peso = 83
    imc = peso / altura ** 2;

if (imc < 1.85){
    console.log(`IMC: ${imc} -- Abaixo do peso`);
} else if (imc >= 18.5 && imc < 24.9){
    console.log(`IMC: ${imc} -- Peso normal`)
} else if (imc >= 25.o && imc < 29.9) {
    console.log(`IMC: ${imc} -- Sobrepeso`)
} else if (imc >= 30.o && imc < 34.9)
console.log(`IMC: ${imc} -- Obesidade grau I`)
} else if (imc >= 35.o && imc < 39.9)
console.log(`IMC: ${imc} -- Obesidade grau II`)
} else {
console.log(`IMC: ${imc} -- Obesidade III`)
}

~~~

Teste 3:

~~~js

const =
    altura = 1.73
    peso = 83
    imc = 24.91;

if (imc < 1.85){
    console.log(`IMC: ${imc} -- Abaixo do peso`);
} else if (imc >= 18.5 && imc < 25.0){
    console.log(`IMC: ${imc} -- Peso normal`)
} else if (imc >= 25.o && imc < 30.0) {
    console.log(`IMC: ${imc} -- Sobrepeso`)
} else if (imc >= 30.o && imc < 35)
console.log(`IMC: ${imc} -- Obesidade grau I`)
} else if (imc >= 35.o && imc < 40.0)
console.log(`IMC: ${imc} -- Obesidade grau II`)
} else {
console.log(`IMC: ${imc} -- Obesidade III`)
}
~~~
