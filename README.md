# wordpress-development-livraira

Certifiquese que tem um cliente docker instalado
 > Recomendado colima (rancher desktop pode ser instalado para ter a sintaxe do cli do docker mais atual)
```shell
brew install colima docker docker-compose
brew install kubectl
# Recursos padrão: 2CPUs, 2GB de memória, 60GB de storage e sem kubernetes
colima start

# Personalizando recursos
colima stop
colima start --cpu 2 --memory 4 --disk 60 --with-kubernetes
```

## Prepare
Se estiver com processador arm (Mac M1) nenhum paço a mais
Se estiver usando processador x86 (tradicional) remova `arm64v8/` do docker file

## Start Up
```shel
make start
```
caso seja a primeira vez que está rodando
```shell
make first-start
```

Parar container
```shell
make stop
```

---

## Como Usar
Instale os pluguins e themas desejados na pasta e seja feliz
