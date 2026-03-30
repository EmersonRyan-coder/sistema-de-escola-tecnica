# Modelagem Conceitual

Esse documento descreve as entidades e seus relacionamentos no sistema.

## O diagrama foi desenvolvido utilizando draw.io.
![Diagrama](../diagrama_v1.jpeg)

Este diagrama representa a estrutura de um sistema de escola técnica, focado na visão do aluno. Partes como administrativas e outras foram abstraídas.

O foco deste diagrama é compreender como as entidades se relacionam no sistema.


## 📌 Observações:
- As PKs estão destacadas em verde.
- As FKs estão destacadas em roxo.
- A explicação foca nas entidades, atributos e relacionamentos, sem detalhar as chaves primárias.

# Explicação das entidades

 ## Aluno
### Descrição: Representa o estudante no sistema.
### Atributos:
- Nome
- CPF
- Data de nascimento
- Telefone
- E-mail
- Endereço

 ## Matrículas
Relaciona o aluno a uma turma.
### Atributos:
- FK ID aluno: Identificador do aluno
- FK ID turma: Identificador da turma
- Data da matrícula: Data que foi criada a matrícula
- Status: Indica se a matrícula está Ativa, Trancada, Em espera ou Cancelada
  ### Observações:
- A matrícula serve para vincular os alunos com as turmas. O curso não foi incluído na matrícula, pois já está vinculado à turma, evitando redundância de dados.

 ## Professores
### Descrição: Representa o professor no sistema.
### Atributos:
 - Nome
 - CPF
 - Telefone
 - E-mail
 - Especialidade: Área de atuação ou formação
 
  ## Cursos
### Descrição: Representa os cursos oferecidos na instituição.
Um curso pode possuir várias turmas.
Um curso pode possuir várias matérias.
### Atributos:
- Nome: Nome de cada curso
- Carga horária: Quantas horas o curso tem no total
- Início: Data de início do curso
- Término: Data de fim de curso
 
## 🚨 Em desenvolvimento
A documentação ainda não está completa.
As explicações e alterações serão adicionadas progressivamente.
