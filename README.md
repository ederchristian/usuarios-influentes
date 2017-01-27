# Usuários Influentes 1.0

Este webapp visa entender melhor o perfil de usuários influentes em diferentes setores.

[Link do webapp]

### Utilizando o Apache

* [Faça o download] ou instale:
    * No macOS
        ```sh
        $ sudo su -
        $ apachectl start
        ```
    * No Linux
         ```sh
        $ sudo apt-get update
        $ sudo apt-get install apache2
        ```
    * [No Windows]
    
* Configure os arquivos no macOS:
    ```sh
    $ cd /etc/apache2/users
    $ sudo nano username.conf
    ```

    No prompt de comando:
    ```sh
    <Directory "/Users/username/Sites/">
        AllowOverride All
        Options Indexes MultiViews FollowSymLinks
        Require all granted
    </Directory>
    ```

    Trocar "username" pelo nome do usuário da máquina.

[Link do webapp]: <http://ederchristian.com/usuarios-influentes>
[Faça o download]: <https://www.apache.org/dyn/closer.cgi>
[No Windows]: <https://httpd.apache.org/docs/2.4/platform/windows.html>