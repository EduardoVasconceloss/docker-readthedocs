# Docker ReadTheDocs Tutorial

## Este repositório contém um tutorial detalhado sobre como baixar e configurar o ReadTheDocs usando o Docker.

### Pré-requisitos
Antes de começar, verifique se você possui o Docker instalado em seu sistema. Para instalar o Docker, consulte a documentação oficial em https://docs.docker.com/get-docker/.

## Passo a Passo
### Siga as instruções abaixo para configurar o ReadTheDocs usando o Docker:

- ### Clonar o repositório do Github 
**``git clone https://github.com/EduardoVasconceloss/docker-readthedocs.git``**

- ### Crie um diretório na partição var e mude o nome dele 
**``mkdir rtd && chown -R 1005:205 /var/local/rtd``**

- ### Entre no diretório que você clonou do github e rode esse comando 
**``docker run -it -v /var/local/rtd:/data -p 8001:8000 -e RTD_PRODUCTION_DOMAIN="\<IP-da-máquina\>:8001" -d seblon/readthedocs-docker``**

- ### Agora acesse o ReadTheDocs via navegador 
**``http://\<IP-da-máquina\>:8001``**
##
## Dicas
- Personalize e adicione sua documentação ao projeto.
- Faça um commit das alterações em seu repositório local.
- Publique seu repositório no GitHub.
- Compartilhe seu tutorial com a comunidade e aproveite o ReadTheDocs em um ambiente Docker!

### Contribuição
Se você encontrar algum problema ou tiver sugestões de melhoria, sinta-se à vontade para abrir uma issue ou enviar um pull request.
