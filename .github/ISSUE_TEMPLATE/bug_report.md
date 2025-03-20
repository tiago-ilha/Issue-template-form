name: Bug Report
description: Relate um problema encontrado na aplicação
title: "[BUG]: "
labels: [bug]
body:
  - type: markdown
    attributes:
      value: "Por favor, preencha as informações abaixo para relatar o problema."

  - type: input
    id: sistema-operacional
    attributes:
      label: "Sistema Operacional"
      description: "Qual sistema operacional você está usando?"
      placeholder: "Windows 11, Ubuntu 22.04, etc."

  - type: textarea
    id: descricao
    attributes:
      label: "Descrição do problema"
      description: "Explique o problema encontrado."
      placeholder: "Ocorre um erro ao tentar acessar a funcionalidade X..."
      value: ""

  - type: dropdown
    id: prioridade
    attributes:
      label: "Prioridade"
      description: "Qual a prioridade desse bug?"
      options:
        - Baixa
        - Média
        - Alta
    validations:
      required: true
