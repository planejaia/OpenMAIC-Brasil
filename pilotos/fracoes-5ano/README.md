# Piloto OpenMAIC Brasil — Frações no 5º ano

## Objetivo

Provar, com o mínimo de desenvolvimento, se o OpenMAIC consegue transformar uma habilidade curricular oficial em uma experiência de aprendizagem interativa útil para professores e alunos do 5º ano do Ensino Fundamental.

Este piloto **não altera o núcleo do OpenMAIC**. Primeiro usamos as capacidades que já existem no projeto: geração de curso, professor e colegas de IA, quiz, quadro branco, voz e simulações HTML.

## Recorte inicial

- **Etapa:** Ensino Fundamental — Anos Iniciais
- **Ano:** 5º ano
- **Componente:** Matemática
- **Unidade temática:** Números
- **Tema do piloto:** Frações equivalentes
- **Habilidade de referência:** **EF05MA04**
- **Referências curriculares:** BNCC + Currículo Base da Educação Infantil e do Ensino Fundamental do Território Catarinense

O objetivo operacional do piloto é fazer o aluno reconhecer, construir e justificar equivalências entre frações usando mais de uma representação, em vez de apenas acertar contas mecanicamente.

## Hipótese a testar

Uma única habilidade oficial pode originar muitas trajetórias de aprendizagem sem que seja necessário escrever milhares de exercícios previamente.

O OpenMAIC deve combinar, dinamicamente:

- explicação do professor de IA;
- representação visual (barra, coleção, reta numérica e outros recursos adequados);
- colegas de IA com dúvidas e argumentos diferentes;
- erros conceituais plausíveis para o aluno identificar e corrigir;
- perguntas de justificativa ("como você sabe?");
- quiz de verificação;
- atividade/simulação interativa quando fizer sentido;
- fechamento com evidências de aprendizagem para o professor.

## Regra central do piloto

**A IA não deve apenas dar a resposta.** Ela deve criar situações em que o aluno precise explicar, comparar, representar, corrigir e justificar.

## Experiência mínima esperada

Uma sessão de aproximadamente 20–25 minutos com este fluxo:

1. **Diagnóstico rápido** — descobrir o que o aluno já entende sobre partes de um inteiro.
2. **Exploração visual** — comparar duas representações equivalentes, por exemplo 1/2 e 2/4.
3. **Discussão multiagente** — um colega de IA apresenta um raciocínio correto e outro apresenta um erro plausível.
4. **Aluno argumenta** — escolhe, explica e corrige quando necessário.
5. **Nova representação** — trabalhar a mesma ideia em outro contexto/visual.
6. **Desafio adaptativo** — dificuldade muda conforme a resposta do aluno.
7. **Quiz curto** — verificar se a equivalência foi compreendida em situações novas.
8. **Fechamento** — síntese do que foi demonstrado e do que ainda precisa ser trabalhado.

## Critério de sucesso do MVP

O piloto é promissor se professores, após testarem uma aula gerada, responderem positivamente a três perguntas:

1. **Está matematicamente correto?**
2. **Está alinhado ao que um aluno do 5º ano precisa aprender?**
3. **Eu usaria ou adaptaria isto em uma aula real?**

A primeira validação deve ser feita com professores/adultos, sem dados pessoais de crianças reais.

## O que NÃO faremos nesta fase

- criar um novo LMS ou ERP escolar;
- reescrever a interface do OpenMAIC;
- cadastrar escolas, turmas ou alunos reais;
- treinar um modelo próprio;
- reproduzir livro didático comercial;
- criar milhões de perguntas previamente;
- automatizar avaliação oficial de alunos.

## Arquivos deste piloto

- [`prompt-openmaic.md`](./prompt-openmaic.md) — instrução pronta para gerar a primeira aula no OpenMAIC.
- [`plano-de-teste.md`](./plano-de-teste.md) — checklist para professores avaliarem a experiência.
- [`materiais/README.md`](./materiais/README.md) — fontes curriculares e regras de uso dos materiais.

## Próxima decisão após o teste

Só depois de observar a aula gerada decidiremos se alguma adaptação de código é realmente necessária. Se o OpenMAIC original resolver bem o caso, o próximo investimento deve ser em **conteúdo, validação pedagógica e experiência do professor**, não em reconstruir a plataforma.