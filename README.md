## Como Configurar o Projeto

Caso você prefira rodar o projeto utilizando Docker e Dev Container, siga os passos abaixo

Passo 1 - Clonar o Repositorio do Github.

Comando:
```
git clone https://github.com/franciscorjr/claude-course.git
```

Passo 2 - Criação de Arquivo .env usando o .env.example, nesse passo você deverá informa sua ANTHROPIC_API_KEY dentro das aspas duplas do arquivo .env que foi gerado após a execução do compando `cp`

Comando:
```
cp .env.example .env
```

Passo 3 - Subir o container e fazer o build da imagem

Comando:
```
docker compose up --build
```

Passo 4 - Acessar a aplicação via navegador no endereço `http://localhost:8888/`

Você deverá ser capaz de ver essa tela

![alt text](/imgs-docs/image-1.png)

Passo 5 - OPCIONAL:  necessita ter a extenção do `Dev Containers` da Microsoft instalado no seu VS Code

Caso você queria utilizar o notebook via VS Code e via navegador ao mesmo tempo

O projeto está configurado para que você possa utilizar o VS Code através do Dev Container

Onde o VS Code é executado dentro de um container seperado e não na sua máquina

Para fazer isso bastar subir os container normalmente através do comando

Comando:
```
docker compose up -d
```

Após o container estiver rodando, vá até o canto inferior esquerdo do seu VS Code e clique nesse icone <>

![alt text](/imgs-docs/image-2.png)

após clicar será exebido um wizard no VS Code parecido com esse

![alt text](/imgs-docs/image-3.png)

Selecione a opção: `Reopen in Container` e espere o VS Code reiniciar

Pronto agora você poderá utilizar o notebook dentro do container e também no navegador

Observe o canto inferior esquerdo da imagem abaixo, ele indica que o VS Code está rodando dentro do `Dev Container: Claude Course`

![alt text](/imgs-docs/image-4.png)
