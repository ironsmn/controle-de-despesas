# Documento de consulta do sistema

Este documento resume o funcionamento do sistema **CDD - Controle de Despesas**. Ele serve como apoio para entender a navegação, as telas disponíveis, as ações principais e as tecnologias usadas no projeto.

## Objetivo do sistema

O CDD é um sistema web para controle financeiro pessoal. Ele permite registrar receitas e despesas, acompanhar o saldo, consultar transações e visualizar relatórios financeiros.

Nesta versão acadêmica, o sistema funciona no front-end e salva os dados no navegador usando `localStorage`.

## Como navegar no site

A navegação principal do sistema acontece por meio do menu lateral, exibido após o login.

As principais áreas disponíveis são:

- **Painel Financeiro**
- **Transações**
- **Relatórios**
- **Gerenciar Perfil**

Antes do login, o usuário tem acesso à tela inicial, ao cadastro de usuário e à recuperação de senha simulada.

## Telas disponíveis

### Tela inicial

Tela de entrada do sistema.

Ações disponíveis:

- acessar o sistema por login;
- abrir a tela de cadastro;
- abrir a recuperação de senha simulada.

### Cadastro

Tela usada para criar uma conta de usuário.

Ações disponíveis:

- informar nome completo;
- informar e-mail;
- criar senha;
- confirmar senha;
- salvar os dados do usuário no navegador;
- voltar para a tela inicial.

### Recuperação de senha

Modal usado para simular a recuperação de senha.

Ações disponíveis:

- informar e-mail;
- simular o envio de link de recuperação;
- fechar o modal.

### Painel Financeiro

Tela principal do sistema após o login.

Ações disponíveis:

- visualizar saldo atual;
- visualizar total de receitas;
- visualizar total de despesas;
- filtrar informações por data;
- filtrar por categoria de receita;
- filtrar por categoria de despesa;
- limpar filtros;
- consultar gráficos financeiros.

### Transações

Tela usada para gerenciar receitas e despesas.

Ações disponíveis:

- cadastrar nova receita;
- cadastrar nova despesa;
- editar transação existente;
- excluir transação;
- buscar por descrição;
- filtrar por tipo;
- filtrar por categoria;
- filtrar por período;
- limpar filtros.

Ao editar uma transação, o tipo original é mantido. Uma receita continua sendo receita, e uma despesa continua sendo despesa.

### Relatórios

Tela usada para consultar informações financeiras em forma de resumo e gráficos.

Ações disponíveis:

- selecionar o ano do relatório;
- visualizar total de receitas no ano;
- visualizar total de despesas no ano;
- visualizar saldo do ano;
- consultar gráfico mensal de receitas e despesas;
- consultar gráfico de despesas por categoria;
- consultar tabela de categorias.

### Gerenciar Perfil

Tela usada para alterar dados do usuário.

Ações disponíveis:

- visualizar nome e e-mail do usuário;
- alterar nome;
- alterar e-mail;
- alterar telefone;
- alterar moeda;
- alterar formato de data;
- alterar senha de forma simulada;
- salvar alterações no navegador.

## Armazenamento dos dados

O sistema usa `localStorage`, que é um recurso do navegador para salvar dados localmente.

Dados armazenados:

- dados do usuário;
- receitas;
- despesas;
- versão dos dados de exemplo.

Essa escolha foi usada porque o projeto é uma versão acadêmica front-end. Assim, não é necessário configurar banco de dados ou servidor externo nesta etapa.

## Tecnologias utilizadas

- **React:** usado para construir as telas e componentes do sistema.
- **React Router:** usado para controlar a navegação entre as páginas.
- **TypeScript:** usado para organizar melhor o código e reduzir erros simples.
- **Vite:** usado para executar o projeto durante o desenvolvimento e gerar a versão final.
- **CSS Modules:** usado para separar os estilos por tela ou componente.
- **Recharts:** usado para criar os gráficos do painel e dos relatórios.
- **Tabler Icons:** usado para exibir ícones nas telas.
- **Radix UI Dialog:** usado como base para modal de forma acessível.
- **localStorage:** usado para salvar dados no navegador.

## Limitações atuais

- O login é simulado.
- A recuperação de senha é simulada.
- Os dados ficam salvos apenas no navegador usado.
- Não há banco de dados externo.
- Não há API própria.
- Não há integração com banco, Pix, cartão ou serviço financeiro.

## Possíveis melhorias futuras

- Criar autenticação real.
- Integrar banco de dados.
- Criar uma API para salvar e consultar dados.
- Publicar o sistema em ambiente online.
- Permitir exportação de relatórios.
