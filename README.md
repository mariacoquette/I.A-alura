const caixaPrincipal = document.querySelector(".caixa-principal");
const caixaPerguntas = document.querySelector(".caixa-perguntas");
const caixaAlternativas = document.querySelector(".caixa-alternativas");
const caixaResultado = document.querySelector(".caixa-resultado");
const textoResultado = document.querySelector(".texto-resultado");

const perguntas = [
    {
        enunciado: "Como transformar meu gato femea em macho?",
        alternativas: [
            "Alternativa 1",
            "Alternativa 2"
        ]
    },
    {
        enunciado: "Pergunta 2",
        alternativas: [
            "Alternativa 1",
            "Alternativa 2"
        ]
    }
];
let atual = 0;
let perguntaAtual;

function mostrarPergunta() {

   perguntaAtual = pergunta(atual);
   caixaPerguntas.texteContent = perguntaAtual.enunciado;
   
}

mostrarPergunta()
