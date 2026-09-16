# Plano de teste — Piloto Frações 5º ano

## Objetivo do teste

Avaliar se uma aula gerada pelo OpenMAIC a partir da habilidade **EF05MA04 — identificar frações equivalentes** é correta, adequada ao 5º ano e útil para um professor real.

Nesta fase, o teste deve ser feito primeiro com **adultos/professores**, sem cadastro ou dados pessoais de crianças.

## Como executar

1. Abrir o OpenMAIC.
2. Selecionar português do Brasil.
3. Usar o conteúdo de `prompt-openmaic.md` como instrução de geração.
4. Se o ambiente permitir anexos, fornecer somente as referências curriculares oficiais indicadas em `materiais/README.md`.
5. Gerar uma aula de aproximadamente 20–25 minutos.
6. Percorrer a aula inteira como se fosse um aluno do 5º ano.
7. Testar pelo menos três comportamentos do aluno:
   - resposta correta com boa justificativa;
   - resposta errada típica;
   - resposta incompleta ou “não sei”.
8. Registrar o que o sistema fez em cada situação.

## Cenários mínimos

### Cenário A — compreensão correta

Aluno reconhece que `1/2 = 2/4` e consegue explicar usando uma representação visual.

**Esperado:** o sistema reconhece a justificativa e propõe um desafio um pouco mais complexo, sem repetir desnecessariamente a explicação básica.

### Cenário B — erro por comparação de números isolados

Aluno afirma que `2/4 > 1/2` porque 2 é maior que 1.

**Esperado:** o sistema não apenas marca como errado. Deve provocar comparação visual ou fazer perguntas que ajudem o aluno a perceber que as duas frações representam a mesma quantidade.

### Cenário C — erro envolvendo denominador

Aluno afirma que `1/8 > 1/4` porque 8 é maior que 4.

**Esperado:** o sistema ajuda a distinguir “quantidade de partes” de “tamanho de cada parte”.

### Cenário D — resposta sem justificativa

Aluno responde corretamente, mas apenas escreve `3/6 = 1/2`.

**Esperado:** o sistema pede explicação, desenho, comparação ou outra evidência de compreensão.

### Cenário E — não sei

Aluno responde “não sei”.

**Esperado:** o professor de IA oferece uma pista simples e gradual, sem entregar imediatamente a resposta final.

## Ficha de avaliação do professor

Dar nota de **1 a 5** para cada item.

| Critério | 1 | 2 | 3 | 4 | 5 |
|---|---:|---:|---:|---:|---:|
| Correção matemática | | | | | |
| Adequação ao 5º ano | | | | | |
| Clareza da linguagem | | | | | |
| Qualidade das representações visuais | | | | | |
| Qualidade das perguntas do professor IA | | | | | |
| Qualidade dos erros/dúvidas dos colegas IA | | | | | |
| Capacidade de reagir ao erro do aluno | | | | | |
| Estímulo à explicação e argumentação | | | | | |
| Utilidade para uma aula real | | | | | |
| Interesse/engajamento provável do aluno | | | | | |

## Três perguntas decisivas

Ao final, perguntar ao professor:

1. **Você usaria esta experiência com seus alunos?** — Sim / Não / Com alterações.
2. **O que você precisaria mudar antes de usar?**
3. **Esta ferramenta economizaria seu tempo ou criaria mais trabalho? Por quê?**

## Falhas graves

Qualquer uma destas falhas deve ser registrada separadamente:

- erro matemático;
- afirmação curricular inventada;
- feedback que reforça um raciocínio incorreto;
- conteúdo incompatível com a faixa etária;
- resposta excessivamente longa ou confusa;
- entrega da resposta sem oportunidade de raciocínio;
- simulação visual inconsistente com a matemática;
- insistência em uma trajetória quando o aluno já demonstrou domínio.

## Critério inicial de avanço

Não é uma validação científica. É um filtro de MVP.

Avançar para um piloto maior apenas se:

- não houver erros matemáticos graves nas sessões avaliadas;
- a média de **correção matemática** for pelo menos 4/5;
- a média de **adequação ao 5º ano** for pelo menos 4/5;
- ao menos 2 de 3 professores disserem que usariam a experiência ou usariam com pequenas alterações.

Se esses critérios não forem atendidos, corrigir primeiro prompts, fontes e comportamento do OpenMAIC antes de desenvolver novas funcionalidades.