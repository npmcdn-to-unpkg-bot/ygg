Definição as URLs e Respostas da API REST 
---
Versão 1.0 

Neste documento serão definidas as URLs para utilização na aplicação, seus parâmetros e suas respostas.
As requisições e respostas seguem o padrão definido no documento de [Definições](https://github.com/gabrielbo1/ygg/blob/master/Documentos/YGG_DEFN_1.1_20160511.md Definições).

#### URLs disponíveis

##### Definição da URL Base

A `URL Base` é o caminho padrão para a realização das requisições. 
A URL é composta pela concatenação da `URL Base` com o nome da função, segue exemplo:

`http://urlbaseprojeto.com.br/rest/funcionalidade`

**Valor da URL Base:** `http://ygg.pe.hu/rest`

##### Definição das URLs

`http://ygg.pe.hu/rest/cadastro`

Método: _POST_

Função responsável por realizar o cadastro de um usuário no sistema sem ser através das redes sociais.

|Parâmetros|Tipo|
|----------|-------|
|Nome      | _String_ |
|email     | _String_|
|senha     | _String_|

`http://ygg.pe.hu/rest/cadastroRedeSocial`

Método: _POST_

Função responsável por realizar o cadastro de um usuário no sistema através das Redes Sociais Facebook ou Google+

*A Definir*

`http://ygg.pe.hu/rest/login`

Método: _GET_

Função responsável por realizar a autenticação dos dados de um usuário cadastrado via YGG.

|Parâmetros| Tipo|
|----------|--------|
|email     |_String_|
|senha     |_String_|

`http://ygg.pe.hu/rest/loginRedeSocial`

Método: _GET_

Função responsável por realizar a autenticação de um usuário cadastrado via Redes Sociais.

*A Definir*

`http://ygg.pe.hu/rest/usuario`

Método: _GET_

|Parâmetros| Tipo|
|----------|--------|
|usID      | _Integer_|
|sessionID | _String_|

`http://ygg.pe.hu/rest/apagar`

Função responsável por alterar a situação de um usuário para **excluido**.

|Parâmetros|Tipo|
|----------|-----|
|usID      |_Integer_|


`http://ygg.pe.hu/rest/atualizarPerfil`

Método: _POST_

Função responsável por atualizar o perfil de um usuário.

|Parâmetros| Tipo |
|-----------|------|
|usID | _Integer_|
|usNome|_String_|
|usEmail|_Strign_|