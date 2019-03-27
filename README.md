## SSH-Ubuntu
Feito para comunicação com servidor, usando SSH (OpenSSH).  

#### Comandos
---- 
para que você possa se conectar inicie o comando abaixo em seu console.
```sh
$ ssh -i "arquivo-config" "user"
```
para listar os arquivos do servidor use.
```sh
$ ls
$ ls -la # ocultos
```
para escolher a pasta
```sh
$ cd "pasta"
```
copiar pasta dentro do servidor
```sh
$ sudo cp -r "pasta-original" "pasta-salvar"
```
copiar pasta do computador para o servidor
```sh
$ scp -r -i "arquivo-config" "pasta-a-enviar" "user":"pasta-a-receber"
```

#### Comando para editar arquivos
----
abrir arquivo
```sh
$ sudo vi "arquivo" 
```
no arquivo aperte **i** você vai pode fazer alteraçes nele.
para salvar aperte: ``` Shift+: ``` e digite **wq**.
pronto o arquivo estara salvo.

#### Procurar arquivo no servidor
----
selecione a pasta usando os comandos acima, logo apos use:
```sh
$ find . -name "nome-do-arquivo.php"
```
