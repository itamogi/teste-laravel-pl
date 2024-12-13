# Teste Prático - Desenvolvedor Pleno (PHP/Laravel)

## Objetivo

O objetivo deste teste é avaliar suas habilidades em PHP, Laravel, MySQL, HTML, CSS, JavaScript e integração de APIs, com foco na API do Mercado Livre. Este teste inclui desafios de desenvolvimento backend e frontend, bem como o consumo e manipulação de dados em tempo real usando a API oficial do Mercado Livre.

---

## Cenário

Você foi contratado para desenvolver um sistema de gestão de vendas no Mercado Livre. Esse sistema deve permitir o cadastro de produtos, a sincronização do estoque e a atualização de preços. Também deve exibir os pedidos recebidos em tempo real, utilizando Webhooks.

---

## Desafio 1: Cadastro e Atualização de Produtos

Crie um sistema em Laravel que permita realizar o cadastro e a atualização de produtos na API do Mercado Livre.

### Requisitos:

1. Crie um formulário para o cadastro e a edição de produtos com os seguintes campos:
   - Nome
   - Descrição
   - Preço
   - Quantidade em estoque
   - Categoria (busque as categorias da API do Mercado Livre)
   - Imagens (upload de múltiplas imagens)

2. Ao cadastrar ou editar um produto, envie as informações para a API do Mercado Livre e salve os dados no banco de dados local (MySQL).

3. Utilize a funcionalidade de "atributos" da API do Mercado Livre para cadastrar produtos em categorias que exigem informações adicionais, como cor, tamanho, etc.

4. Exiba a resposta retornada pela API (código do produto, status, erros, etc.) em um painel de administração simples.

---

## Desafio 2: Sincronização de Estoque e Preços

Implemente uma funcionalidade para sincronizar automaticamente o estoque e os preços dos produtos cadastrados com a API do Mercado Livre.

### Requisitos:

1. Crie uma rotina agendada utilizando o **Scheduler** do Laravel para:
   - Atualizar o estoque de todos os produtos com base nos dados armazenados no banco local.
   - Atualizar o preço de produtos com base em promoções configuradas.

2. Certifique-se de registrar logs das atualizações realizadas.

---

## Desafio 3: Recebimento de Pedidos

Implemente um sistema para exibir pedidos recebidos em tempo real utilizando Webhooks da API do Mercado Livre.

### Requisitos:

1. Configure um endpoint para receber notificações de pedidos (Webhooks).

2. Salve os dados dos pedidos recebidos no banco de dados, incluindo:
   - ID do pedido
   - Nome do comprador
   - Produtos adquiridos
   - Preço total
   - Status do pedido

3. Crie uma página no sistema que exiba a lista de pedidos.

---

## Desafio 4: Documentação

Crie um arquivo `README.md` com as seguintes informações:

1. Instruções detalhadas sobre como instalar e rodar o projeto.
2. Como configurar as variáveis de ambiente para a integração com o Mercado Livre (client_id, client_secret, redirect_uri, etc.).
3. Passos detalhados para configurar Webhooks no Mercado Livre.
4. Como executar o Scheduler do Laravel para sincronização de estoque e preços.

---

## Bônus (Opcional)

- Implemente autenticação no sistema utilizando **Laravel Breeze** ou **Laravel Jetstream**.
- Crie testes automatizados para as funcionalidades principais (ex.: cadastro de produtos, sincronização de estoque, recebimento de pedidos).
- Use **Docker** para configurar o ambiente de desenvolvimento.
- Utilize um framework CSS moderno como Tailwind ou Bootstrap para criar uma interface amigável e responsiva.

---

## O que será avaliado:

1. Organização do código e boas práticas em PHP e Laravel.
2. Implementação da integração com a API do Mercado Livre.
3. Validação e tratamento de erros na comunicação com a API.
4. Utilização de recursos modernos do Laravel (Scheduler, WebSockets, etc.).
5. Interface funcional e bem estruturada.

---

Após finalizar o projeto, suba o código em um repositório público no GitHub e envie um e-mail para **psymics@gmail.com** com a URL do repositório.

**Boa sorte!**
