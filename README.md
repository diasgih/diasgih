## Hi 👋

// Array de objetos representando alunos e suas notas
const alunos = [
  { nome: 'Ana', notas: [8, 9, 7, 6] },
  { nome: 'João', notas: [5, 7, 8, 6] },
  { nome: 'Carlos', notas: [9, 8, 9, 10] },
  { nome: 'Bianca', notas: [7, 8, 6, 7] }
];

// Função para calcular a média
const calcularMedia = (notas) => {
  let soma = 0;
  notas.forEach((nota) => {
    soma += nota;
  });
  return soma / notas.length;
};

// Usando forEach para percorrer a lista de alunos e mostrar o nome e a média de cada um
alunos.forEach((aluno) => {
  const media = calcularMedia(aluno.notas);
  console.log(`Aluno: ${aluno.nome} | Média: ${media.toFixed(2)}`);
});
