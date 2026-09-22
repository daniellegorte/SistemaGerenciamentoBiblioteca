# Sistema de Gerenciamento de Biblioteca

O projeto tem como objetivo o gerenciamento de uma biblioteca, por meio de controle e acesso a dados relacionados a livros e usuários de maneira acessível e intuitiva.


## Tecnologias Utilizadas
<div> C# (Windows Form) | MySQL Workbench | Xampp | Visual Studio </div>



## Requisitos para funcionamento
### Instalação do Software XAMPP e MySQL Workbench
* Em **XAMPP Control Panel** Iniciar o módulo **"MySQL"**;
* Em **MySQL Connections** acessar o servidor local ou criar novo e configurar:

   **Connection Name:** _nomeDesejado_

   **Hostname:** 127.0.0.1

   **Port:** _porta indicada pelo XAMPP_

   **Username:** root

* Criar Banco de Dados nomeado 'biblioteca';
* Executar script de criação e população do Banco de Dados;

### Conectando o sistema com Banco de Dados
* Com o o projeto "P1 - Gerenciamento de Biblioteca" aberto no *Visual Studio*, clique com o botão direito em "*Referências*" e selecione “**Manage NuGet Packages (Gerenciar Pacotes do NuGet).**”
* Na aba *Browse*, pesquise por **MySql.Data** , selecione o pacote oficial da Oracle e clique em Install;
* Na classe “Conexao.cs”, na linha do construtor (public Conexao()):

  ``` String dataSource = "datasource=localhost; username = root; password = '';" + "database='biblioteca';AllowZeroDateTime=true;";> ```

  **password:** Deixe em branco ("") se o **XAMP** estiver com a senha padrão.

  **database:** Caso necessário, altere de 'biblioteca' para o nome do banco de dados criado.

**OBS:** Para a conexão ser válida e realizada, é necessário que os módulos “MySQL” esteja iniciado no **XAMPP**, com o status em verde. 


