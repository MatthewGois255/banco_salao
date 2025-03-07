![docker-mysql](https://github.com/user-attachments/assets/b97f6e1a-acf9-4620-9104-c31eb3800263)
### Docker commands
~~~
docker pull mysql
~~~
Make sure you've created a folder to store the Database's volume. In my case, it's "~/dados-mysql"
~~~
docker run --name bancosalao -e MYSQL_ROOT_PASSWORD=123bancoSalao -v ~/dados-mysql:/var/lib/mysql -p 3280:3306 -d mysql
~~~

### Enabling Port Forwarding in VirtualBox

Settings > Network > Port Forwarding > add rule (at the top right side)

Host IP = 127.0.0.1 <br>
Host Port = 3280 <br>
Guest IP = 10.0.2.15 <br>
Guest Port = 3280

![pf](portforwarding.png)

### Creating Database

I'm using MySQL Workbench for connecting to the database

The SQL script is [here](script.sql)

The Modeling file is [here](bancosalao.mwb)

### Queries


