<p>Uma Promise é um objeto que representa a eventual conclusão ou falha de uma operação assíncrona.<br></p>
<p> As Promises têm três estados possíveis: pendente, resolvida e rejeitada<br></p>
<p>exemplos de uma promise rejeitada seguir:</p>


const promessaRejeitada = new Promise((resolve, reject) => {
  setTimeout(() => {
    reject("Promessa rejeitada!");
  }, 1000);
});

promessaRejeitada
  .then(resultado => {
    console.log(resultado);
  })
  .catch(erro => {
    console.error(erro);
  });