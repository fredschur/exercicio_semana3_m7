Este código é uma aplicação PHP simples para gerenciar reservas em um restaurante. Ele permite que os usuários insiram detalhes de uma reserva e exibe todas as reservas em uma tabela.

# Funcionalidades

Conexão com o Banco de Dados: O código se conecta a um banco de dados MySQL usando as credenciais fornecidas em ../inc/dbinfo.inc.
Verificação da Tabela: Verifica se a tabela "RESERVATIONS" existe no banco de dados e a cria se não existir.
Adicionar Reserva: Os usuários podem adicionar uma reserva fornecendo o nome do cliente, informações de contato, data da reserva e número de convidados.
Exibir Reservas: Todas as reservas são exibidas em uma tabela HTML.

# Estrutura da Tabela

A tabela "RESERVATIONS" tem a seguinte estrutura:
ID: Chave primária, autoincremento.
NAME: Nome do cliente (VARCHAR 45).
CONTACT: Informações de contato do cliente (VARCHAR 45).
DATE: Data da reserva (DATE).
GUESTS: Número de convidados (INT 4).

# Como Usar
Certifique-se de que o arquivo ../inc/dbinfo.inc contém as credenciais corretas para o seu banco de dados MySQL.
Coloque este arquivo PHP em seu servidor web.
Acesse o arquivo através do navegador e utilize o formulário para adicionar reservas.
As reservas existentes serão exibidas abaixo do formulário.
