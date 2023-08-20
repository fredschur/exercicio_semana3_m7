# Página de Produtos

Este script PHP fornece uma interface web para gerenciar produtos dentro de um banco de dados. Ele permite que os usuários adicionem novos produtos e visualizem os existentes.

# Recursos

Conexão com Banco de Dados MySQL: Utiliza o MySQL para armazenar e recuperar informações de produtos.
Adicionar Novos Produtos: Os usuários podem adicionar novos produtos fornecendo detalhes como nome, descrição, preço e categoria.
Listar Produtos Existentes: Exibe uma tabela com todos os produtos existentes no banco de dados.
Validação de Entrada: Garante que a entrada seja devidamente tratada para evitar injeção de SQL.
Verificação de Tabela: Verifica se a tabela de produtos existe no banco de dados e a cria, se não existir.

# Requisitos

PHP 5.5 ou superior
MySQL 5.6 ou superior
Arquivo de configuração do banco de dados (../inc/dbinfo.inc)

# Uso

Configuração do Banco de Dados: Certifique-se de que o arquivo de configuração do banco de dados (../inc/dbinfo.inc) esteja configurado corretamente com as credenciais do banco de dados (DB_SERVER, DB_USERNAME, DB_PASSWORD, DB_DATABASE).

Acessar a Página: Abra o arquivo PHP em um navegador web.

Adicionar um Produto: Preencha os detalhes do produto no formulário fornecido e clique no botão "Adicionar Produto".

Visualizar Produtos: Os produtos existentes serão listados em uma tabela abaixo do formulário.

# Funções

AddProduct($connection, $name, $description, $price, $category): Adiciona um novo produto ao banco de dados.
VerifyProductsTable($connection, $dbName): Verifica se a tabela de produtos existe e a cria, se não existir.
TableExists($tableName, $connection, $dbName): Verifica se uma tabela existe no banco de dados.
