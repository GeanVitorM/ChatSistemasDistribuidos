# ChatSignalR

## Descrição

O **ChatSignalR** é uma aplicação de chat em tempo real construída com **ASP.NET Core** e **SignalR**. Permite que múltiplos usuários se conectem ao chat, enviem mensagens para todos os participantes ou para usuários específicos. Está configurada para ser acessível a partir de qualquer dispositivo na rede local, utilizando o endereço IP da máquina onde o servidor está rodando.

## Tecnologias Utilizadas

- **ASP.NET Core 5.0 ou superior**: Framework para construção de aplicações web.
- **SignalR**: Biblioteca para comunicação em tempo real entre cliente e servidor.
- **Bootstrap 4.4.1**: Framework CSS para estilização da interface do usuário.
- **JavaScript/jQuery**: Para manipulação do DOM e envio de mensagens através do SignalR.
- **NoSQL Database (opcional)**: Para armazenamento de mensagens enviadas no chat.

## Pré-requisitos

- **.NET 5.0 ou superior**: [Instale o SDK .NET](https://dotnet.microsoft.com/download).
- **Visual Studio 2019/2022 ou VS Code**: IDE recomendada para desenvolvimento em C#.
- **Node.js (opcional)**: Para gerenciamento de pacotes front-end, se desejar usar npm para instalar bibliotecas.

## Instalação

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/SeuUsuario/ChatSignalR.git
   cd ChatSignalR
Instale as dependências:

Certifique-se de que o .NET SDK está instalado na sua máquina:

   ```bash
      Copiar código
   ```
      dotnet restore

**Configure o ambiente**:

## Se necessário, configure as variáveis de ambiente ou altere as configurações no arquivo appsettings.json.

**Compile e execute o projeto:**

   ```bash
   dotnet build
   dotnet run
   ```
**Acesse a aplicação:**

## A aplicação estará disponível em http://<SeuIPLocal>:5001. Utilize o endereço IP local da sua máquina para que outros dispositivos na rede possam acessar o chat.

## Como Funciona
-- **Chat em Tempo Real: Usuários podem enviar mensagens para todos os participantes ou diretamente para um usuário específico.**
-- **Armazenamento de Mensagens: O código está preparado para integrar com um banco de dados NoSQL para armazenar as mensagens, mas essa funcionalidade pode ser customizada conforme necessário.**
-- **Acesso Local: A aplicação está configurada para ser acessível a partir de qualquer dispositivo na rede local.**
-- **Estrutura do Projeto**
-- **ChatSignalR.Hubs/ChatHub.cs: Contém a lógica do Hub SignalR para gerenciar as conexões e mensagens do chat.**
-- **Startup.cs: Configura os serviços necessários, incluindo SignalR.**
-- **Program.cs: Configura o servidor para ouvir em todas as interfaces de rede.**
