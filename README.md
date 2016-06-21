# Disponibilidade NET #

Exemplo de utilização da API Javascript do Google Maps para plotar informações sobre disponibilidade de instalação da NET (www.netcombo.com.br) em uma determinada rua a partir da consulta de CEP da mesma.

###Requisitos

Chave válida da API:

https://developers.google.com/maps/documentation/javascript/get-api-key

### Endpoints

Consulta de CEP JSON gratuita a partir de um nome de rua, cidade e estado:

https://viacep.com.br/ws/**ESTADO**/**CIDADE**/**RUA**/json/

Consulta de disponibilidade do site oficial da NET retornando um JSONP com um booleano dado um CEP:

http://programacao.netcombo.com.br/gatekeeper/cep/select?wt=jsonp&rows=1&json.wrf=parseAddress&indent=true&fl=cep,grupo,uf,cidade,bairro,via,hasNet&q=cep%3A**CEP**&true=parseAddress

### Utilização

Clique sobre uma rua e aguarde a informação ser exibida.

Caso a consulta de CEP não esteja disponível na rua ou não haja disponibilidade mensagens correspondentes são exibidas.

Caso haja mais de uma rua com o mesmo nome, todos os ceps e respectivos nomes e bairros são exibidos.

