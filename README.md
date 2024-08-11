ChatSignalR
Descrição
O ChatSignalR é uma aplicação de chat em tempo real construída com o ASP.NET Core e SignalR. Este projeto permite que múltiplos usuários se conectem ao chat, enviem mensagens para todos os participantes ou mensagens diretas para um usuário específico. A aplicação é configurada para permitir que qualquer pessoa na rede local acesse o chat através do endereço IP da máquina onde o servidor está rodando.

Tecnologias Utilizadas
ASP.NET Core 5.0 ou superior: Framework para construção de aplicações web.
SignalR: Biblioteca para comunicação em tempo real entre cliente e servidor.
Bootstrap 4.4.1: Framework CSS para estilização da interface do usuário.
JavaScript/jQuery: Para manipulação do DOM e envio de mensagens através do SignalR.
NoSQL Database (opcional): Para armazenamento de mensagens enviadas no chat.
Pré-requisitos
.NET 5.0 ou superior: Instale o SDK .NET.
Visual Studio 2019/2022 ou VS Code: IDE recomendada para desenvolvimento em C#.
Node.js (opcional): Para gerenciamento de pacotes front-end se desejar usar npm para instalar bibliotecas.
Instalação
Clone o repositório:

bash
Copiar código
git clone https://github.com/SeuUsuario/ChatSignalR.git
cd ChatSignalR
Instale as dependências:

Certifique-se de que o .NET SDK está instalado na sua máquina:

bash
Copiar código
dotnet restore
Configure o ambiente:

Se necessário, configure as variáveis de ambiente, ou altere as configurações no arquivo appsettings.json.

Compile e execute o projeto:

bash
Copiar código
dotnet build
dotnet run
Acesse a aplicação:

A aplicação estará disponível em http://<SeuIPLocal>:5001. Utilize o endereço IP local da sua máquina para que outros dispositivos na rede possam acessar o chat.

Como Funciona
Chat em Tempo Real: Os usuários podem enviar mensagens para todos os participantes ou diretamente para um usuário específico.
Armazenamento de Mensagens: O código está preparado para integrar com um banco de dados NoSQL para armazenar as mensagens, mas essa funcionalidade pode ser customizada conforme necessário.
Acesso Local: A aplicação está configurada para ser acessível a partir de qualquer dispositivo na rede local.
Estrutura do Projeto
ChatSignalR.Hubs/ChatHub.cs: Contém a lógica do Hub SignalR para gerenciar as conexões e mensagens do chat.
Startup.cs: Configura os serviços necessários, incluindo SignalR.
Program.cs: Configura o servidor para ouvir em todas as interfaces de rede.
Uso
Inicie a aplicação na sua máquina local.
Acesse o chat utilizando o endereço IP da máquina e a porta configurada (por padrão, 5001).
Insira seu apelido, escolha um destinatário e envie sua mensagem.
Personalização
Porta: Para alterar a porta em que a aplicação escuta, modifique a linha webBuilder.UseUrls("http://*:5001"); no arquivo Program.cs.
Estilo CSS: O estilo da aplicação é baseado em Bootstrap, mas pode ser personalizado conforme necessário.
Contribuição
Se você encontrar bugs ou quiser contribuir com melhorias, fique à vontade para abrir uma issue ou enviar um pull request.

Licença
Este projeto é distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
