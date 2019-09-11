
## Processo de CI - 11/09/2019

Nessa fase, você deverá repetir o processo ensinado no módulo.

1) Você deverá pegar sua aplicação Laravel das fases anteriores e adicioná-la em um pipeline de integração contínua utilizando o Google Cloud Build, para isso terá que:


    - Gerar a imagem do docker-compose e fazer o push no seu Container Registry do GCP. 

    - Criar uma trigger para ser disparada todas as vezes que um commit entrar no repositório do Github.

    Os steps do Google Cloud Build deverão ser:

        - Executar o docker-compose
        - Executar o composer
        - Copiar o arquivo .env.example para .env
        - Rodar um artisan key:generate
        - Executar as migrações
        - Executar os testes utilizando o PHPUnit

2) Você deverá instalar a App do Google Cloud Build disponível no Market Place do Github. Crie um branch develop em seu repositório. Todas as vezes que uma pull request for criada, imediatamente o Google Cloud Build deverá iniciar o processo de CI.

## Docker Hub

- [marcoskubas/laravel-docker](https://hub.docker.com/r/marcoskubas/laravel-docker)

## Desafio Docker

2) Esse desafio é muito empolgante principalmente se você nunca trabalhou com a linguagem Go!
Você terá que publicar uma imagem no docker hub. Quando executarmos:

docker run <seu-user>/codeeducation 

Temos que ter o seguinte resultado: Code.education Rocks!

Se você perceber, essa imagem apenas realiza um print da mensagem como resultado final, logo, vale a pena dar uma conferida no próprio site da Go Lang para aprender como fazer um "olá mundo".

Lembrando que a Go Lang possui imagens oficiais prontas, vale a pena consultar o Docker Hub.

3) A imagem de nosso projeto Go precisa ter menos de 2MB =)

Dica: No vídeo de introdução sobre o Docker quando falamos sobre o sistema de arquivos em camadas, apresento uma imagem "raiz", talvez seja uma boa utilizá-la.

Divirta-se

# Docker Hub e Repositório GitHub

https://hub.docker.com/r/marcoskubas/codeeducation

https://github.com/marcoskubas/gocodeeducation

