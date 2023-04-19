# JobRotation
Job Rotation - Ribeirão Preto

Questão nº1 - Resposta:  Valor da váriavel é 91.

Questão nº2 - Resposta: // Definindo o número a ser verificado
const numeroVerificar = 12;

// Definindo as duas primeiras posições da sequência
let fib1 = 0;
let fib2 = 1;

// Verificando se o número informado é 0 ou 1 (casos base da sequência)
if (numeroVerificar === 0) {
  console.log("O número 0 pertence à sequência de Fibonacci.");
} else if (numeroVerificar === 1) {
  console.log("O número 1 pertence à sequência de Fibonacci.");
} else {
  // Calculando a sequência de Fibonacci até o número informado ou até ultrapassá-lo
  let fibAtual = fib1 + fib2;
  while (fibAtual <= numeroVerificar) {
    if (fibAtual === numeroVerificar) {
      console.log(`O número ${numeroVerificar} pertence à sequência de Fibonacci.`);
      break;
    }
    fib1 = fib2;
    fib2 = fibAtual;
    fibAtual = fib1 + fib2;
  }

  // Verificando se o número informado não pertence à sequência
  if (fibAtual > numeroVerificar) {
    console.log(`O número ${numeroVerificar} não pertence à sequência de Fibonacci.`);
  }
}

Questão nº 3 - Resposta: a) 9 b) 128 c) 49 d) 100 e) 13 f) 20

Questão nº 4 - Resposta:

// Definindo as constantes de distância e velocidade
const distanciaTotal = 100; // Distância entre as cidades em km
const velocidadeCarro = 110; // Velocidade do carro em km/h
const velocidadeCaminhao = 80; // Velocidade do caminhão em km/h

// Calculando o tempo de encontro dos veículos
const tempoEncontro = distanciaTotal / (velocidadeCarro + velocidadeCaminhao);

// Calculando as distâncias percorridas por cada veículo até o ponto de encontro
const distanciaCarro = velocidadeCarro * tempoEncontro;
const distanciaCaminhao = (velocidadeCaminhao * tempoEncontro) + (0.0833 * 2); // Considerando 2 pedágios de 5 minutos cada

// Calculando a distância de cada veículo até Ribeirão Preto
const distanciaRibeiraoPretoCarro = distanciaTotal - distanciaCarro;
const distanciaRibeiraoPretoCaminhao = distanciaCaminhao;

// Verificando qual veículo está mais próximo de Ribeirão Preto
let veiculoMaisProximo = "";
if (distanciaRibeiraoPretoCarro < distanciaRibeiraoPretoCaminhao) {
  veiculoMaisProximo = "o carro";
} else {
  veiculoMaisProximo = "o caminhão";
}

// Imprimindo o resultado
console.log(`Quando se cruzarem na rodovia, ${veiculoMaisProximo} estará mais próximo de Ribeirão Preto.`);

Questão nº 5 - Resposta:  
let palavra = "100";
let invertida = "";

for (let i = palavra.length - 1; i >= 0; i--) {
  invertida += palavra[i];
}

console.log(invertida); // imprime "001"

