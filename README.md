# Carona UCB 🚗🎓

## 📖 Visão Geral
Este projeto trata-se de um trabalho acadêmico desenvolvido com o objetivo de avaliar a capacidade dos alunos em executar uma Sprint simulada e validar, na prática, os conhecimentos em métodos ágeis. O objeto de estudo desta simulação é o **Carona UCB**, uma proposta de aplicativo de caronas solidárias voltado para alunos, professores e servidores de um mesmo campus universitário.

## 🎯 Problema e Objetivo
*   **Problema:** Alta dependência de transporte público e uso de meios informais para compartilhamento de caronas sem controle de segurança, registro de rotas ou garantia de vínculo institucional.
*   **Usuário Principal:** Estudantes, professores e demais funcionários da Universidade.
*   **Sprint Goal:** Validar o fluxo principal do CaronaUCB, permitindo que a comunidade acadêmica consiga se cadastrar, oferecer, buscar e solicitar caronas com segurança.

## 🚀 Funcionalidades da Sprint Inicial (Backlog)
Para validar o fluxo principal (Sprint Goal), foram selecionadas 4 histórias de usuário (User Stories), totalizando 26 Story Points:

*   **Cadastro Institucional (US1 - 5 Pontos):** Apenas pessoas vinculadas à instituição podem acessar o aplicativo. O sistema bloqueia cadastros de domínios que não sejam da universidade e envia um link de validação para o e-mail.
*   **Oferta de Vagas (US2 - 8 Pontos):** O motorista cadastra a rota com origem, destino, data, horário e quantidade de assentos. A carona fica disponível no sistema imediatamente após ser salva.
*   **Busca de Caronas (US3 - 8 Pontos):** Pesquisa filtrada por horário e proximidade. O tempo de resposta deve ser estritamente inferior a 2 segundos em Android e iOS, omitindo caronas que já estejam lotadas.
*   **Solicitação de Vaga (US4 - 5 Pontos):** O motorista recebe a notificação da solicitação, e a vaga fica com o status "pendente" até a aprovação.

## 🔜 Próximas Funcionalidades (Sprints Futuras)
Outras histórias foram mantidas na coluna *To Do* por excederem a capacidade da equipe e não impedirem a validação do fluxo principal nesta primeira Sprint:

*   **Sistema de Avaliação (US5 - 5 Pontos):** Ativação de uma tela de avaliação de 1 a 5 estrelas quando o horário da viagem for atingido. Avaliações abaixo de 2 estrelas exigem uma justificativa obrigatória em um campo de texto.
*   **Privacidade e Exclusão de Dados (US6 - 3 Pontos):** Um código rodará diariamente para limpar os registros de localização com mais de 90 dias, registrando a exclusão em um arquivo.
*   **Gestão de Solicitações (US7 - 3 Pontos):** Ao aceitar a solicitação, o número de vagas da carona diminui em 1 e o passageiro é notificado da resposta.
*   **Chat Temporário (US8 - 8 Pontos):** Chat interno ativado apenas após o status da carona mudar para "Aceita". O histórico é apagado 24 horas após o fim da viagem para garantir a segurança.

## 🛠 Metodologia de Trabalho (Kanban e Qualidade)
A gestão da Sprint foi realizada com metodologias ágeis através do Trello:

*   **Quadro Kanban:** Dividido nas colunas *To Do*, *Doing*, *Testing / Code Review* e *Done*.
*   **Limite de Work in Progress (WIP):** Estabelecido em um máximo de duas tarefas simultâneas para as colunas *Doing* e *Testing / Code Review*, com o intuito de impedir que a equipe inicie diversas atividades ao mesmo tempo, evitando gargalos e perda de foco.
*   **Definition of Done (DoD):** Um cartão só vai para a coluna final (*Done*) se o código for testado em Android e iOS, todos os critérios de aceitação validados e os rigorosos requisitos de segurança da universidade respeitados.

## 📈 Métricas e Aprendizados da Equipe
*   A equipe utilizou um *Burndown Chart* de 20 dias que projetou a entrega inicial dos 26 Story Points.
*   Entre o décimo primeiro e o décimo quarto dia, o fluxo enfrentou um bloqueio severo na coluna *Testing / Code Review* provocado por problemas complexos de validação na US2 e atrasos de informações por parte do setor de TI da UCB.
*   Ao respeitar os limites de WIP (máximo de 2 tarefas na coluna de testes), o problema travou o avanço de novos cartões, forçando toda a equipe a se concentrar na resolução do gargalo da US2, que só foi resolvido no décimo sétimo dia.
*   **Aprendizados:** A experiência demonstrou a necessidade de mapear detalhadamente os cenários de testes no planejamento para aprimorar as estimativas técnicas. Acima de tudo, validou-se o poder dos limites visuais de Kanban, que transformaram um problema técnico em algo visível, forçando a colaboração da equipe e prevenindo o acúmulo de erros.
