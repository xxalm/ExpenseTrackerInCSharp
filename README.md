# Expense Tracker

Expense Tracker é uma aplicação web desenvolvida em ASP.NET Core para gerenciar transações financeiras. A aplicação permite adicionar, editar, visualizar e excluir transações, além de fornecer gráficos para visualização de despesas e receitas.

## Funcionalidades

- Adicionar, editar e excluir transações.
- Visualizar transações recentes.
- Ver gráficos de despesas por categoria e comparação de receitas e despesas.
- Interface amigável e responsiva.

## Tecnologias Utilizadas

- ASP.NET Core
- Entity Framework Core
- SQLite
- Syncfusion (para gráficos e componentes UI)
- Bootstrap (para estilização)

## Instalação e Execução

### Requisitos

- .NET SDK 6.0 ou superior

### Passos

1. Clone o repositório:
   ```sh
   git clone https://github.com/xxalm/ExpenseTrackerInCSharp.git
   cd ExpenseTrackerInCSharp
   ```
2. Restaure os pacotes NuGet:
   ```sh
   dotnet restore
   ```
3. Aplique as migrações e atualize o banco de dados:
   ```sh
   dotnet ef database update
   ```
4. Execute a aplicação:
   ```sh
   dotnet run
   ```
5. Abra o navegador e acesse:
   ```sh
   http://localhost:5000
   ```

## Publicação

Para publicar a aplicação como um executável self-contained, siga os passos abaixo:

### Passos para Publicação

1. Abra um terminal ou prompt de comando.

2. Navegue até o diretório raiz do projeto.

3. Execute o seguinte comando para publicar a aplicação:

   ```sh
   dotnet publish -c Release -r win-x64 --self-contained
   ```

   Este comando cria uma versão compilada da aplicação que é independente do ambiente .NET instalado no sistema do usuário. O parâmetro -r win-x64 especifica que a publicação deve ser para plataformas Windows de 64 bits. Você pode ajustar esse parâmetro conforme necessário para outras plataformas suportadas pelo .NET SDK.

4. Após a conclusão do comando, os arquivos publicados estarão localizados no diretório `bin\Release\net6.0\win-x64\publish` (considerando que você está usando o SDK .NET 6.0 e o .NET Core 6.0).

5. Distribua os arquivos gerados para outros usuários, incluindo o executável principal `ExpenseTracker.exe`.
   

### Executando o Aplicativo Publicado

Para executar o aplicativo publicado em um ambiente Windows:

1. Navegue até o diretório onde os arquivos foram publicados.

2. Execute o arquivo `ExpenseTracker.exe` clicando duas vezes sobre ele, ou abrindo-o via linha de comando.

3. O aplicativo iniciará e estará pronto para uso.

## Estrutura do Projeto

- **Controllers:** Contém os controladores MVC para gerenciar as requisições.
- **Models:** Contém as classes de modelo que representam os dados da aplicação.
- **Views:** Contém as views Razor para renderizar a interface do usuário.
- **wwwroot:** Contém os arquivos estáticos, como CSS, JavaScript e imagens.
- **Data:** Contém a classe `ApplicationDbContext` que gerencia a interação com o banco de dados.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
