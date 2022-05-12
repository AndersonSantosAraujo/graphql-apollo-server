Playground Tests Querys

query {
  user(id: 5) {
    nome
    role {
      type
    }
  }
}

query {
  users {
    nome
    role {
      type
    }
  }
}

mutation{
  adicionaUser(nome: "Anderson", ativo: true, email: "anderson@gmail.com", role: "ESTUDANTE") {
    nome
    role {
      type
    }
  }
}

mutation {
  atualizaUser(id: 7, nome: "Anderson", ativo: true, email: "anderson@gmail.com", role: "DOCENTE") {
    nome
    role {
      type
    }
  }
}

mutation {
  deletaUser(id: 7)
}

mutation{
  adicionaUser(nome: "Akira", ativo: true, email: "akira@gmail.com", role: COORDENACAO, createdAt: "2022-05-12") {
    nome
    role {
      type
    }
  }
}

mutation {
  adicionaUser(user: {
    nome: "Joana",
    ativo: true,
    email: "joana@gmail.com",
    role: ESTUDANTE,
    createdAt: "2022-05-12"}) {
    nome 
  }
}

mutation {
  atualizaUser(
    id: 11,
    user: {
    nome: "Jaqueline",
    ativo: true,
    email: "joana@gmail.com",
    role: ESTUDANTE,
    createdAt: "2022-05-12"}) {
    nome 
  }
}

mutation {
  atualizaUser(
    id: 11,
    user: {
    nome: "Matilde",
    ativo: true,
    email: "jaqueline@gmail.com",
    role: ESTUDANTE,
    createdAt: "2022-05-12"}) {
    code 
    mensagem
    user {
      nome
    }
  }
}

mutation {
  deletaUser(id: 11) {
    code
    mensagem
  }
}
