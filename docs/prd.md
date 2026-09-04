# 📄 Product Requirements Document (PRD) - Watchlog

## 1. Identificação
- Criador: Leonardo Antunes Domingues da Silva
- Nome da aplicação: Watchlog

## 2. Descrição
O **Watchlog** é uma aplicação web que tem como objetivo auxiliar quem deseja estudar e compreender melhor o mundo de batalhas em duplas do jogo competitivo **Pokémon Champions**, sendo uma opção para que os usuários possam observar e analisar quais times, pokémon e setups que estão sendo utilizados no meta-game atual.

## 2. Atores do Sistema

- **Visitante:** Usuário não autenticado que acessa a página inicial e pode observar um pouco das informações, mas é necessário logar para ter o acesso completo.
- **Cliente:** Usuário autenticado que possui um login e pode ver e analisar todas as estatísticas livremente.

## 3. Histórias de Usuário e Escopo

Abaixo estão as funcionalidades principais do MVP (Minimum Viable Product), escritas sob a perspectiva do usuário final.

**👤 Épico 1: Autenticação e Acesso**
- **US01 - Cadastro de Usuário:** Como um Visitante, quero preencher um formulário com meus dados para criar uma conta na aplicação e ter acesso às informações competitivas.
  _Critérios de Aceitação:_ Todos os campos obrigatórios devem ser preenchidos; o sistema deve validar os dados informados; o usuário deve ser cadastrado com sucesso quando as informações forem válidas.
- **US02 - Acesso ao Sistema (Login):** Como um Usuário cadastrado, quero inserir meu e-mail e senha para acessar as informações completas da aplicação.
  _Critérios de Aceitação:_ O sistema deve validar as credenciais informadas; caso sejam inválidas, deve apresentar uma mensagem de erro; usuários não autenticados não devem ter acesso às informações protegidas.
- **US03 - Encerrar Sessão (Logout):** Como um Usuário logado, quero encerrar minha sessão para sair da aplicação com segurança.
  _Critérios de Aceitação:_ Ao realizar o logout, o usuário deve perder o acesso às áreas protegidas e ser direcionado para a tela de login.
  
**🏆 Épico 2: Pokémon no Meta**

- **US04 - Visualização de Pokémon no Meta:** Como um Usuário logado, quero visualizar os Pokémon mais utilizados no competitivo de duplas para conhecer os principais Pokémon presentes no meta.
  _Critérios de Aceitação:_ A aplicação deve apresentar uma lista de Pokémon; cada Pokémon deve apresentar sua porcentagem de utilização e imagem; os dados devem ser apresentados de forma organizada.
- **US05 - Visualização de Informações do Pokémon:** Como um Usuário logado, quero selecionar um Pokémon do meta para conhecer suas principais características e estatísticas competitivas.
  _Critérios de Aceitação:_ O sistema deve apresentar informações como porcentagem de utilização, movimentos, habilidades e itens mais utilizados, quando disponíveis.
- **US06 - Pesquisa de Pokémon:** Como um Usuário logado, quero pesquisar um Pokémon pelo nome para encontrar rapidamente suas informações competitivas.
  _Critérios de Aceitação:_ O sistema deve permitir a pesquisa pelo nome; caso nenhum Pokémon seja encontrado, deve apresentar uma mensagem informativa.
  
**🧩 Épico 3: Times no Meta**

- **US07 - Visualização de Times no Meta:** Como um Usuário logado, quero visualizar os times mais utilizados no competitivo de duplas para conhecer as principais composições do cenário competitivo.
  _Critérios de Aceitação:_ A aplicação deve apresentar uma lista de times; cada time deve apresentar os Pokémon que fazem parte da composição e sua utilização.
- **US08 - Visualização de Detalhes do Time:** Como um Usuário logado, quero selecionar um time para conhecer sua composição completa e suas informações competitivas.
  _Critérios de Aceitação:_ O sistema deve apresentar os seis Pokémon que compõem o time e as informações disponíveis sobre sua utilização.
  
**🥇 Épico 4: Resultados de Torneios**

- **US09 - Visualização de Torneios:** Como um Usuário logado, quero visualizar os torneios competitivos para acompanhar os principais eventos do cenário competitivo.
  _Critérios de Aceitação:_ O sistema deve apresentar uma lista de torneios com informações como nome, data e local, quando disponíveis.
- **US10 - Visualização de Resultados:** Como um Usuário logado, quero selecionar um torneio para visualizar seus principais resultados e colocações.
Critérios de Aceitação: O sistema deve apresentar os jogadores ou equipes participantes e suas respectivas colocações.
