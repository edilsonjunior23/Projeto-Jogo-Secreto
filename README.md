# Projeto-Jogo-Secreto
Esse foi um código que criei na aula de Java Script.

alert ('bem vindo ao jogo do número secreto');
let numeroSecreto = parseInt(Math.random() * 100 + 1);
console.log (numeroSecreto);
prompt ('escolha um número entre 1 e 100');
let chute;
let tentativas = 1;

// enquanto chute nao for igual ao numero secret
while (chute != numeroSecreto) {
    chute = prompt ('escolha um número enrte 1 e 100');
// se chute for igual ao numero secreto
if (chute == numeroSecreto) {
    break

}
else {
    if (chute > numeroSecreto) {
        alert(`o número é menor que o ${chute}`);
    } else {
        alert(`o número é maior que o ${chute}`);
    }
        // tentativas = tentativas +1
        tentativas++;
    }
}
// if (tentativas > 1) {
//     alert(`Isso ai! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} tentativas.`);
// } else {
//     alert(`Isso ai! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} tentativa.`);
// }
let palavraTentativa = tentativas > 1 ? 'tentativas' : 'tentativa';
alert(`Isso ai! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} ${palavraTentativa}.`);
