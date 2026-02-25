# 💸 App de Organização de Finanças Pessoais com Vibe Coding: "Bate Papo Financeiro"

Este repositório contém o projeto desenvolvido no desafio "Vibe Coding: Criando um App de Finanças Pessoais com IA" da DIO em parceria com a Caixa Econômica Federal.
O app foi criado utilizando o Lovable AI e o Copilot, seguindo o conceito de desenvolvimento orientado por conversas (Vibe Coding), sem escrever código manualmente.

---

## 1. PRD (Prompt Final) utilizado para gerar o app

PRD – App de Organização de Finanças Pessoais Conversacional (com Design Universal)

1. Contexto
O aplicativo será um organizador financeiro baseado em conversas, permitindo que o usuário registre gastos, acompanhe metas e receba orientações de forma natural, sem depender de formulários complexos ou planilhas. A proposta é transformar o controle financeiro em algo simples, acessível e guiado por um “Agente Financeiro” inteligente.

O app deve adotar princípios de design universal, garantindo que pessoas com diferentes níveis de habilidade, experiência, limitações físicas, cognitivas ou sensoriais possam utilizá-lo com conforto e autonomia.

2. Problema
A maioria dos apps de finanças exige preenchimento manual, categorização repetitiva e interfaces pouco intuitivas. Isso leva muitos usuários, especialmente iniciantes, a desistirem do controle financeiro.

O app busca resolver isso oferecendo:
- Registro por linguagem natural
- Automação de classificação
- Recomendações personalizadas
- Experiência fluida e conversacional
- Acessibilidade integrada desde o início

3. Público-Alvo
- Pessoas que querem começar a organizar suas finanças
- Usuários que se frustram com apps tradicionais
- Pessoas que preferem interagir por chat
- Iniciantes em educação financeira
- Usuários que precisam de uma interface acessível e inclusiva

4. Proposta de Valor
Um app que entende o usuário, registra suas transações automaticamente e oferece dicas práticas, tudo por meio de uma conversa simples e amigável, com uma experiência inclusiva e acessível.

5. Funcionalidades-Chave

5.1 Registro de Gastos via Chat
- Usuário digita frases como: “Gastei 35 reais com almoço hoje.”
- O sistema interpreta valor, categoria e data automaticamente.
- Possibilidade de confirmar, editar ou excluir via chat.

5.2 Classificação Automática
- Identificação automática de categorias.
- Sugestões de correção.
- Aprendizado com o uso.

5.3 Metas Financeiras
- Criação de metas simples.
- Acompanhamento via chat e gráficos simples.

5.4 Agente Financeiro
- Dicas personalizadas com base no comportamento do usuário.
- Sugestões de economia e alertas de gastos.
- Linguagem educativa e acessível.

5.5 Relatórios Simples
- Resumo semanal e mensal.
- Gráficos de gastos por categoria.
- Saldo do período.
- Alternativas textuais para gráficos.

6. Requisitos Não Funcionais

6.1 Acessibilidade e Design Universal
- Totalmente utilizável via chat.
- Contraste adequado e tipografia legível.
- Suporte a leitores de tela.
- Não depender exclusivamente de cores.
- Linguagem simples e direta.
- Alternativas textuais para gráficos.
- Fluxos curtos e de baixa carga cognitiva.

6.2 Outros Requisitos
- Interface minimalista e mobile-first.
- Respostas rápidas do agente.
- Segurança e privacidade dos dados.
- Baixa curva de aprendizado.

7. Fluxo do Usuário (MVP)
1. Onboarding simples e criação de conta.
2. Primeira interação: agente pergunta se o usuário quer registrar um gasto ou definir uma meta.
3. Registro de transações via chat.
4. Dashboard básico com resumo do mês.
5. Criação e acompanhamento de metas.
6. Dicas e recomendações periódicas.

8. MVP – Telas e Recursos Necessários

Telas:
- Tela de Login / Cadastro
- Tela de Chat (principal)
- Dashboard simples
- Tela de Metas
- Tela de Relatórios

Recursos Técnicos:
- Interpretação de linguagem natural
- Banco de dados para transações e metas
- Classificação automática por regras simples
- Lógica de recomendações básicas
- Gráficos simples com alternativas textuais

9. Esboço de Validação Inicial
- Testar com 3 a 5 usuários iniciantes.
- Observar:
  - Facilidade para registrar gastos
  - Clareza das respostas do agente
  - Compreensão do dashboard
  - Utilidade das metas
  - Acessibilidade para diferentes perfis de usuários
- Ajustar linguagem, categorias e fluxo com base no feedback.

10. Entregável da IA
Gerar:
- Estrutura do MVP
- Telas essenciais
- Fluxos conversacionais
- Lógica básica de classificação
- Sugestões de melhorias
Com tom educativo e acessível, em português.

---

## 2. Prompts iniciais gerados no Copilot para construir o MVP (7 prompts estratégicos para otimizar interações no Lovable)

### Prompt 1 — Criar o app inteiro baseado no PRD
Quero criar um aplicativo de Organização de Finanças Pessoais baseado em conversas. Use o PRD abaixo como referência completa e obrigatória para toda a construção do app:

{PRD}

Crie o projeto inicial com:
- Tela principal de chat
- Navegação configurada
- Arquitetura organizada
- Componentes básicos reutilizáveis
- Design universal e acessibilidade aplicados desde o início

Não implemente funcionalidades complexas ainda. Apenas a estrutura, layout e navegação.

### Prompt 2 — Implementar o chat funcional
Agora implemente a tela de chat como a interface principal do app.

Requisitos:
- Enviar e receber mensagens
- Simular respostas do Agente Financeiro
- Input acessível
- Layout limpo e responsivo
- Preparado para integrar lógica de interpretação de texto

Não implemente ainda o registro de gastos. Apenas o chat funcional.

### Prompt 3 — Interpretação de linguagem natural + registro de gastos
Implemente a funcionalidade de registrar gastos via linguagem natural.

Regras:
- O usuário envia frases como “Gastei 35 reais com almoço hoje”.
- O sistema deve extrair valor, categoria e data.
- Salvar a transação no banco local.
- Confirmar a interpretação via chat.
- Permitir corrigir ou excluir via chat.

Use lógica simples baseada em padrões de texto.

### Prompt 4 — Banco de dados e modelos
Crie o banco de dados local e os modelos necessários para:

- Transações (valor, categoria, data, descrição, tipo)
- Metas financeiras
- Preferências do usuário

Implemente persistência, carregamento automático e integração com o chat.

### Prompt 5 — Dashboard completo
Crie o dashboard com:

- Total gasto no mês
- Total recebido
- Saldo
- Gráfico de pizza por categoria
- Lista das últimas transações

Garanta que o dashboard leia os dados reais do banco.

### Prompt 6 — Metas financeiras + Agente Financeiro
Implemente:

1. Metas financeiras:
   - Criar metas via chat
   - Salvar metas
   - Mostrar progresso no dashboard
   - Alertas quando o usuário se aproximar do limite

2. Agente Financeiro:
   - Dicas automáticas baseadas no comportamento
   - Alertas de gastos acima da média
   - Tom educativo e acessível

### Prompt 7 — Relatórios + revisão final
Crie a tela de relatórios com:
- Gastos por categoria
- Evolução mensal
- Comparação entre meses
- Alternativas textuais para gráficos

Depois, faça uma revisão geral:
- Ajuste layout
- Padronize componentes
- Melhore acessibilidade
- Otimize performance
- Garanta que o fluxo do usuário esteja claro

Não adicione novas funcionalidades além disso.

---

## 3. Prompts de refinamento utilizados diretamente no Lovable (com auxílio do Copilot na estratuturação):

### Prompt 1 - Implemente um onboarding conversacional no app, integrado à tela de chat.

Requisitos:
O onboarding deve ocorrer apenas na primeira abertura do app.
O Agente Financeiro deve guiar o usuário de forma simples e acessível.

Fluxo do onboarding:
Cumprimento inicial e explicação rápida do funcionamento.
Perguntar o nome do usuário e salvar no banco/local storage.
Perguntar o orçamento mensal aproximado e salvar.
Guiar o usuário para registrar o primeiro gasto com um exemplo.
Registrar esse primeiro gasto usando a lógica já existente.
Encerrar o onboarding com uma mensagem clara e acolhedora.
O onboarding deve ser totalmente conversacional, sem telas extras.
O agente deve usar linguagem simples, inclusiva e acessível.
Após o onboarding, o app deve funcionar normalmente.
Nas próximas aberturas, o onboarding não deve aparecer.
Garanta que o código fique organizado e fácil de manter.
Mantenha o estilo e a arquitetura já criados no projeto, mantendo todo o restante como está

### Prompt 2 - Adicione ao app uma tela inicial de autenticação simples, sem alterar nada já desenvolvido.

Requisitos:

Criar uma tela inicial com:
Botão “Entrar”
Botão “Criar conta”
Link “Esqueci minha senha”
Layout simples, acessível e consistente com o design atual.

Criar a tela de cadastro:
Campos: nome, email, senha
Validação básica
Salvar o usuário no banco/local storage
Após cadastro, redirecionar para o onboarding conversacional já existente.

Criar a tela de login:
Campos: email e senha
Validação simples
Autenticação local (não precisa backend)
Redirecionar para o chat principal após login.

Criar a tela de recuperação de senha:
Campo de email
Exibir mensagem de instrução simples (não precisa enviar email real)
Retornar para a tela de login.

Garantir:
Navegação fluida entre as telas
Acessibilidade (labels, contraste, navegação clara)
Nenhuma alteração na lógica do chat, onboarding ou banco de dados já implementados.
Manter a arquitetura e estilo do projeto.

### Prompt 3 - Adicione ao app um menu acessível e simples, sem alterar nenhuma funcionalidade já implementada.

Requisitos:
Criar um botão de menu (hambúrguer ou similar) visível na interface principal após o login.
Ao abrir o menu, exibir as seguintes opções:
Chat
Dashboard
Metas
Relatórios
Sair

Cada item deve navegar para as telas já existentes, sem modificar o fluxo atual do chat.

A opção “Sair” deve:
Encerrar a sessão do usuário
Limpar o estado de autenticação
Redirecionar para a tela de login

O menu deve seguir princípios de acessibilidade:
Labels claros
Navegação simples
Contraste adequado
Fácil uso com leitores de tela
Não alterar a lógica do chat, onboarding, banco de dados ou telas já criadas.

Manter a arquitetura e o estilo visual do projeto.

### Prompt 4 - Tinha me cadastrado e agora testei cadastrando mais um usuário. Coloquei a mesma senha para o novo usuário e o app acatou. Ao entrar com este novo usuário, as informações de resumo, metas e relatórios ficaram a mesma do meu usuário criado antes, mesmo difitando novas informações nas interações com o chat logado com o novo usuário. Será que foi porque usei a mesma senha? Peço verificar e ajustar.

### Prompt 5 - Corrija e finalize o fluxo de “Esqueci a senha” e revise todo o MVP, sem mudar o escopo do projeto.

Parte 1 – Esqueci a senha:

Implemente o fluxo completo de recuperação de senha:
Ao informar um email cadastrado, simular o envio de um email com instruções de redefinição de senha.
Exibir uma mensagem clara de confirmação, por exemplo: “Enviamos um email com instruções para redefinir sua senha, caso o endereço esteja cadastrado.”
Não é necessário enviar email real, apenas simular o processo.
Após a confirmação de envio:
Redirecionar o usuário para a tela inicial de autenticação (login), e não de volta para “Esqueci a senha”.
Tratar casos de email não cadastrado com mensagem amigável e acessível, sem expor se o email existe ou não no sistema.

Parte 2 – Revisão geral do MVP:

Revise e teste todas as funcionalidades já implementadas, incluindo:
Autenticação:
Cadastro
Login
Logout (Sair)
Esqueci a senha (após correção)

Onboarding conversacional:
Execução apenas no primeiro acesso após login/cadastro
Coleta de nome e orçamento
Registro do primeiro gasto
Integração com o chat principal

Chat:
Envio e recebimento de mensagens
Registro de gastos via linguagem natural
Confirmação, correção e exclusão de transações
Banco de dados:
Persistência de transações, metas e preferências
Carregamento correto ao abrir o app

Dashboard:
Totais (gasto, recebido, saldo)
Gastos por categoria
Últimas transações
Alternativas textuais para gráficos
Metas financeiras:
Criação via chat
Salvamento
Exibição de progresso
Alertas próximos ao limite

Agente Financeiro:
Dicas e alertas baseados em comportamento
Tom educativo, acessível e consistente

Relatórios:
Gastos por categoria
Evolução mensal
Alternativas textuais para gráficos
Menu e navegação:
Menu com opções: Dashboard, Metas, Relatórios, Sair
Navegação fluida entre telas
Sair redirecionando corretamente para a tela de login

Ajuste:
Mensagens de erro e feedback para o usuário, garantindo clareza, simplicidade e acessibilidade.
Pequenos problemas de layout, navegação ou estados quebrados.
Sem adicionar novas funcionalidades além das já previstas no MVP.

Objetivo:
Entregar uma versão final do MVP estável, funcional, acessível e coerente com o PRD.

---

## 4. Imagens ou vídeos das interações com o Copilot e Lovable

Print 1 (Copilot): 
<img width="1356" height="758" alt="image" src="https://github.com/user-attachments/assets/65b7164a-3945-47d0-b8c6-daa05fedaaeb" />

Print 2 (copilot):
<img width="1359" height="764" alt="image" src="https://github.com/user-attachments/assets/38f23fc0-35d5-477f-9bc3-55987a5b781f" />

Print 3 (Copilot):
<img width="1360" height="763" alt="image" src="https://github.com/user-attachments/assets/9c026df4-a24b-4253-ba1a-82dff23a7470" />

Print 4 (Lovable):
<img width="1360" height="767" alt="image" src="https://github.com/user-attachments/assets/1a217fb2-5c84-4e29-bd46-5a0a8b78d3e4" />

Print 5 (Lovable):
<img width="1362" height="767" alt="image" src="https://github.com/user-attachments/assets/12dbd178-5096-4d47-a480-ae32e55c0a4d" />

Print 6 (Lovable):
<img width="1361" height="765" alt="image" src="https://github.com/user-attachments/assets/f89004ec-7d18-4283-95de-109fec812769" />

---

## 5. Resumo do conceito do app

O aplicativo é um organizador de finanças pessoais baseado em conversas.  

O usuário interage com um Agente Financeiro que:
- Registra despesas e receitas via linguagem natural  
- Entende múltiplas transações em uma única mensagem  
- Permite correções inteligentes  
- Cria e acompanha metas financeiras  
- Gera relatórios simples e acessíveis  
- Oferece dicas personalizadas  
- Conduz um onboarding conversacional  
- Segue princípios de design universal e acessibilidade  

O app foi construído inteiramente por prompts, sem programação manual via código.

---

## 6. Reflexão sobre o processo

### O que funcionou bem
- O Lovable interpretou muito bem prompts longos e estruturados.
- Criar o PRD antes acelerou muito o desenvolvimento.
- O chat como interface principal tornou o MVP simples e funcional.
- A IA conseguiu gerar telas, navegação e lógica com poucas interações.

### O que não funcionou como esperado
- A interpretação de linguagem natural exigiu ajustes finos.
- Correções de categorias e múltiplas transações precisaram de prompts específicos.
- O fluxo de "Esqueci a senha" não veio pronto e precisou ser corrigido manualmente via prompt.
- Usuários diferentes inicialmente compartilhavam dados, exigindo correção.

### O que aprendi sobre conversar com IAs
- Quanto mais claro e específico o prompt, melhor o resultado.
- Pedir tudo de uma vez gera resultados piores do que dividir em etapas estratégicas.
- A IA responde melhor quando você explica o contexto e o objetivo final.
- Refinar e iterar faz parte natural do processo — como conversar com um desenvolvedor humano.

---

## 7. Como executar o projeto

O app foi criado no Lovable AI.  
Clique aqui para visualizar o site: https://batepapofinanceiro.lovable.app

---

## 8. Autor

Rafael Francisco Oliveira  
Bootcamp DIO/Caixa Econômica – Vibe Coding

