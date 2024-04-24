Link do classroom: https://classroom.google.com/u/4/c/NjYzMzMyNzc2MzYw

# Contêineres.

## Por que usar contêineres?
Contêineres tornam a aplicação mais:
> - Flexíveis
> - Leves
> - Intercambiáveis
> - Portáteis
> - Escaláveis
> - Empilháveis

## Como funciona um contêiner
Um contêiner é iniciado quando se executa uma **imagem**.

> Imagem: pacote executável que inclui tudo o que é necessário para executar
uma aplicação.
>> Código
Ambiente de execução
Bibliotecas
Variáveis de ambiente
Arquivos de Configuração
Contêiner: instância em execução de uma imagem - o que a imagem se
torna na memória quando executada (imagem, estado, processos).

Diferente de uma _maquina virtual_ o contêiner executa nativamente no Linux e compartilha o kernel da máquina hospedeira com os outros contêineres. Outra vantagem é que cada contêiner executa em um processo separado e por isso não necessita de mais memória do que um processo normal.

Por isso, comparados a maquinas virtuais que executam uma hospedagem completa, contêiner são mais leves.



# Docker.

Docker é uma plataforma de que permite criar e gerenciar contêineres.

## Instalação do docker no linux.
![[docker-deb-install.sh]]

_link da documentação._

## Verificando a versão instalada.
```
docker --version
```

```
docker info
```

> ![[Pasted image 20240314163650.png]]
## Testando a instalação do Docker
```
docker run hello-world
```

> ![[Pasted image 20240314163932.png]]
## Comandos básicos do docker.
- ### Listar imagens instaladas
```
docker image ls
```

> ![[Pasted image 20240314165026.png]]
- ### Listar todos os contêineres
```
docker container ls --all
```

>![[Pasted image 20240314165056.png]]
- ### Listar contêineres em execução
```
docker container ls
```

> ![[Pasted image 20240314165238.png]]
>
> Obs: Nesse caso nenhum contêiner estava sendo executado.

# Criando uma imagem docker
Imagens dockers são criadas usando o arquivos **docker file**. Dentro um **docker file** podemos encontrar:
> - imagem base
> - arquivos
> - volumes persistentes
> - variáveis de ambiente
> - comandos a serem executados na aplicação.

**slide 2**...
# Rodando um projeto com docker
slide 1 pag 10

# Expressões regulares
Recomendação de site: https://regex101.com/

