# Server

1. Instalar o python mais recente (https://www.python.org/downloads/).

2. Adicionar a variável python em PATH (no final da instalação do python ele dá essa opção).

3. Abrir o cmd e instalar o Flask (pip install flask).

4. Descobrir qual o seu IP local pelo cmd (ipconfig) (o endereço certo é o IPV4 Address).

  4.1 Editar a linha 6 do arquivo 'app.py' ('UPLOAD_FOLDER'), com o caminho para a pasta upload do seu computador, caso não seja feito
  o código retornará um erro de arquivo não encontrado.
    
    4.1.2 Copiar o endereço pelo explorer do Windows faz com que as barras fiquem invertidas, é necessário substituir para as barras
    'normais', '\' para '/'.
  
  4.2 Editar a última linha do arquivo 'app.py', no final, onde tem host='192.168...', colocar o seu IP (a alteração pode ser feita pelo bloco de notas).

5. Inicializar o 'app.py'.

6. No navegador, inserir o endereço do seu IP + ':5000' + '/upload'.

7. Inserir o arquivo que deseja fazer o upload e enviar (ainda não da pra enviar mais de um arquivo por vez, ainda).

8. O upload do arquivo é feito pra pasta 'uploads'.

Obs: atualmente, as extensões permitidas para upload são: 'txt', 'pdf', 'png', 'jpg', 'jpeg', 'gif', 'mp4', 'mp3', 'zip', 'rar' e 'exe'.
Caso haja a necessidade de adicionar outras extensões, no arquivo 'app.py' há uma variável chamada 'ALLOWED_EXTENSIONS', basta adicionar
vírgula e o tipo de extensão entre aspas simples.
