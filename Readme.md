# Tecnologias ultilizadas

Aplicação desenvolvida no estudo de docker 

## Docker machine
Docker machine é a ferramenta usada para essa gerência distribuída, permite a instalação e gerência de docker hosts de forma fácil e direta.
Essa ferramenta é muito usada por usuários de sistema operacional “não linux”, como demonstraremos ainda, mas sua função não limita-se a esse fim, pois também é bastante usada para provisionar e gerenciar infraestrutura Docker na nuvem, tal como AWS, Digital Ocean e Openstack.


## Traefik proxy 
O Docker pode ser uma maneira eficiente de executar aplicativos web em produção, mas você pode querer executar vários aplicativos no mesmo host do Docker. Nesta situação, você precisará configurar um proxy reverso, já que você só deseja expor as portas 80 e 443 para o resto do mundo.

O Traefik é um proxy reverso que reconhece o Docker e inclui seu próprio painel de monitoramento ou dashboard. 


Comando para rodar o docker com as configurações do Trafik
```
docker-compose -f docker-compose.yml -f docker-production.yml

```
