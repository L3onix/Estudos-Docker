Para dar deploy neste arquivo ".yml" deverá utilizar um dos 3 comando baixo, dependendo de como pretende rodar o compose.
+ #docker-compose -f docker-compose.yml up
+ #docker stack deploy -c docker-compose.yml compose-tomcat-glassfish

Para testar pode ser acessado pelo navegador utilizando as endereços
+ 0.0.0.0:9000
+ 0.0.0.0:9010
+ 0.0.0.0:9011