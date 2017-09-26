# Gerenciamento de Projetos - Red Hat BPM Suite

## Fluxo
<p><img src="/images/01.png?raw=true"></p>

## Configurações
* Instalação do WebService que será chamado. Neste caso é necessário a instalação de: [https://github.com/kerdlix/ws-rest-random-value](https://github.com/kerdlix/ws-rest-random-value)
* Email Work Item Handler no deployment descriptor
* Necessario iniciar o servidor FakeSMTP como sudo
* Configurar user-info.properties e email.properties
* Documentação: [https://access.redhat.com/solutions/1440913](https://access.redhat.com/solutions/1440913)

## Criação de Usuários
```
./add-user.sh -a --user usuarioPMO         --password redhat@123 --role analyst,pmo
./add-user.sh -a --user usuarioSupervisor  --password redhat@123 --role analyst,supervisor
./add-user.sh -a --user usuarioEngenharia  --password redhat@123 --role analyst,engenharia
./add-user.sh -a --user usuarioSuprimentos --password redhat@123 --role analyst,suprimentos
```


