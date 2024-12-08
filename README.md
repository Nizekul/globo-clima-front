
# Frontend - Aplicação de Favoritos 🌡️☀️🌦️⛈️🌪️

Este é o frontend para a aplicação de favoritos, desenvolvido com Blazor Server. Ele permite que os usuários visualizem, adicionem e removam favoritos, bem como obtenham informações climáticas para os locais favoritos.

## Funcionalidades

- **Listagem de Favoritos**: Exibe uma lista de lugares favoritos com as temperaturas em °C e °F.
- **Exclusão de Favoritos**: Permite ao usuário remover lugares da lista de favoritos.
- **Paginação**: A lista de favoritos pode ser paginada para facilitar a navegação.

## Como Rodar o Frontend

### Pré-requisitos

1. **Instalar o .NET SDK**: 
   - Se ainda não tiver, instale o .NET SDK na sua máquina: [Instalar .NET](https://dotnet.microsoft.com/download/dotnet).

2. **Configuração**:
   - O frontend está configurado para se comunicar com a API: [Api publica](https://github.com/Nizekul/globo-clima) ou no appsettings apontar para a api que esta comentada, porém no futuro esse Ip será desligado.
   - Certifique-se de que a API esteja rodando antes de executar o frontend.

### Rodando o Projeto

1. Clone o repositório.
2. Navegue até o diretório do projeto frontend.
3. Execute o projeto com o comando:

   ```bash
   dotnet run
   ```

   O aplicativo estará disponível em `https://localhost:5208`.

### Estrutura do Projeto

O projeto frontend é composto por componentes em Blazor:

- **`Favorites.razor`**: Página principal que exibe os favoritos e permite a remoção de itens da lista.
- **`Weather.razor`**: Página que mostra os países para poder favoritar, junto com seus climas.

### Como Funciona

- O componente `Favorites.razor` carrega a lista de favoritos do backend, exibe informações como cidade, temperatura e ações para remover os favoritos.
- A interação com o backend é feita por meio de chamadas HTTP, utilizando o `HttpClient` do Blazor.
