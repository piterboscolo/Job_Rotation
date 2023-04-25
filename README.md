# Job_Rotation
Job Rotation - Ribeirão Preto


# Resposta da Questão 1
a variável INDICE é definida como 13, a variável SOMA é definida como 0 e a variável K é definida como 0.

primeira iteração do loop, K é incrementado para 1 e SOMA é atualizado para SOMA + K, ou seja, 0 + 1, resultando em SOMA = 1.

segunda iteração do loop, K é incrementado para 2 e SOMA é atualizado para SOMA + K, ou seja, 1 + 2, resultando em SOMA = 3.

O processo continua até que K seja incrementado para 13 e SOMA seja atualizado para SOMA + K, ou seja, 78.

Após a última iteração do loop, a variável SOMA terá um valor total de 1 + 2 + 3 + ... + 13 = 91.

 o valor da variável SOMA será 91.
 
 

# Resposta da Questão 2)

Em Javascript o código ficaria assim:
````
const num = parseInt(prompt("Informe um número: "));

// Inicialização das variáveis para o cálculo da sequência
let a = 0, b = 1;
const fib = [];

// Loop para gerar a sequência até que o último número seja menor ou igual ao número informado
while (b <= num) {
  fib.push(b);
  [a, b] = [b, a + b];
}

// Verificação se o número informado pertence à sequência
if (fib.includes(num)) {
  console.log(`${num} pertence à sequência de Fibonacci.`);
} else {
  console.log(`${num} não pertence à sequência de Fibonacci.`);
}

````

# Resposta da Questão 3)

a resposta a) Resposta: 1, 3, 5, 7, 9

a resposta b) Resposta: 2, 4, 8, 16, 32, 64, 128

a resposta c) Resposta: 0, 1, 4, 9, 16, 25, 36, 49

a resposta d) Resposta: 4, 16, 36, 64, 100

a resposta e) Resposta: 1, 1, 2, 3, 5, 8, 13

a resposta f) Resposta: 2, 10, 12, 16, 17, 18, 19, 20


# Resposta da Questão 4)

Distância de RP a Franca é de 100km
velocidade do carro é 110km/h para percorrer 50 km ( t = d/v >> t=50km/110km/h = 0,45 horas)
velocidade do caminhão é 80km/h + 5 minutos em cada pedágio, para percorrer 50km (t = d/v + pedagio >> t=50km/80km/h+1/6h = 0,675 horas)

Assim, quando os dois veículos se cruzarem na rodovia, o carro terá percorrido 50 km em 0,45 horas, enquanto o caminhão terá percorrido a mesma distância em 0,675 horas.

podemos calcular a distância entre cada veículo e Ribeirão Preto quando eles se cruzarem. Como eles estarão na mesma distância da cidade, basta subtrair a distância percorrida por cada um a partir de Ribeirão Preto (50 km) para obter a distância restante até a cidade:

distância do carro para Ribeirão Preto = 50 km - 50 km = 0 km
distância do caminhão para Ribeirão Preto = 50 km - 50 km = 0 km


# Resposta da Questão 5)

Javascript
````
let string = prompt("Digite uma string:"); // pode ser substituído por uma string pré-definida no código

// converte a string para uma array de caracteres
let caracteres = string.split("");

// obtém o tamanho da array
let tamanho = caracteres.length;

// itera sobre metade da array e troca os caracteres de posição
for (let i = 0; i < tamanho / 2; i++) {
  let temp = caracteres[i];
  caracteres[i] = caracteres[tamanho - i - 1];
  caracteres[tamanho - i - 1] = temp;
}

// converte a array de volta para uma string
let string_invertida = caracteres.join("");

// imprime a string invertida
console.log("A string invertida é:", string_invertida);
````
