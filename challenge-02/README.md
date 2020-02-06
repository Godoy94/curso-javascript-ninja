# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(x, y){
  return x+y;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
let soma = 5 + soma(1,2);

// Qual o valor atualizado dessa variável?
8

// Declare uma nova variável, sem valor.
let semValor;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function addValor(semValor){
  semValor = 5
  return ("O valor da variavel semValor agora é " + semValor);
}

// Invoque a função criada acima.
addValor()

// Qual o retorno da função? (Use comentários de bloco).
O valor da variável semValor agora é 5

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function verificaValor(x, y, z){
    if(x === '' || y === '' || z === ''){
        alert("Todos os valores devem ser informados");
    } else {
        alert(parseInt(x*y*z+2));
    }
}

verificaValor(1,2,5);

// Invoque a função criada acima, passando só dois números como argumento.
verificaValor(1,2, )

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
Todos os valores devem ser preenchido corretamente

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
verificaValor(1,2,5);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
12

Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.

function master(x, y, z){
    if(x !== undefined && y == undefined && z == undefined){
        return alert(x);
    } else if (x !== undefined && y !== undefined && z == undefined){
        return alert(x + y);
    } else if (x !== undefined && y !== undefined && z !== undefined){
        return alert( (x + y) / z);
    } else if (x == undefined && y == undefined && z == undefined){
        return alert(false);
    } else {
        return alert(null);
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
?
master(1) retorna 1
master(1,1) retorna 2
master(2,2,2) retorna 3
master() retorna false
