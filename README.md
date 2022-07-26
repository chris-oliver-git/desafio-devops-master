desafio-devops-master
Iniciando a analise dos arquivos

Não consegui abrir o app, consegui subir tudo, os containers estão up mas por algum motivo a pasta não é carregada no localhost, bildei as imagens, redefini os parâmetros de porta, sintaxe, identação, criei novas variáveis mas acredito estar faltando algo.

alterações do Dockercompose
> adicionei a lib do mysql
> adicionei a porta 3306 do mysql
> adicionei a variável node networks em networks no modo bridge

alterações na pasta node
> dockerfile 
    > apontei a pasta package.json
    > instalei o npm
    > apontei para salvar as informações em um template
    > adicionei o CMD com as propriedades de execução
> connectionDb
    > faltava algumas pontuações
> Nginx
    > Dockerfile
        > adicionei a pasta config.d onde era para buscar as informações
    > nginx.conf
        adicionei um proxy reverso para mandar as requisições para app
> SQL
    > Dockerfile
        > abri a porta 3306 

No geral, está tudo up, consigo abrir os dockers e editar a pagina inicial mas não consigo abrir o app no navegador.
Estou entregando por causa do prazo mas vou seguir tentando resolver.

Obrigado pela oportunidade.