# Desafio - Instituto CERTI Sapientia

### Servidor HTTP de conversão de números, recebendo um número em algarismo no PATH e retornando no método GET o mesmo número em extenso em um objeto JSON. Os números recebidos podem estar no intervalo [-99.999, 99.999] e retonam em português de acordo com os exemplos a seguir:                         
> $curl http://localhost:5000/39321
>```json
>{
>    "numero": "escreveu 98700",
>    "numero convertido": "noventa e oito mil e setecentos"
>}

> $curl http://localhost:5000/39321
>```json
>{
>    "numero": "escreveu -0111",
>    "numero convertido": "menos cento e onze"
>}

> $curl http://localhost:5000/44g90
>```json
>{
>    "mensagem": "escreva um numero entre -99999 e 99999"
>}

## Executando
### Modo 1:
Baixe o arquivo em .zip e descompacte. Pelo terminal entre no diretório descompactado e ative o ambiente virtual da pasta 'venv'.

Se estiver usando o Windows, abra o terminal PowerShell e execute o seguinte comando para ativar a 'venv':

>python -m venv .\.venv

>.\.venv\Scripts\activate

É possível que o PowerShell precise de uma mudança de permissionamento para execução do 'activate', de acordo com a doc https://docs.microsoft.com/pt-br/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.1 o comando a seguir costuma resolver:

>Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

Quando o ambiente virtual estiver habilitado, aparecerá o nome 'venv' à esquerda de PS no terminal. Então, deverá fazer a instalação dos seguintes pacotes:

> pip install Flask Flask-restful sqlalchemy
> 

Em seguida execute o arquivo 'app.py' com o comando:

>python app.py

Interaja com a API pelo caminho http://localhost:5000/ conforme os exemplos dados.

### Modo 2:
Baixe o arquivo em .zip e descompacte.

Pela IDE PyCharme abra o projeto no diretório de destino. 

O ambiente da 'venv' já deve estar ativado por padrão do projeto. Execute o arquivo 'app.py'. 

Interaja com a API pelo caminho http://localhost:5000/ conforme os exemplos dados.
