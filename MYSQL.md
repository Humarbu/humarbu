**Instal·lació sistema gestor de base de dades. MySQL**


- En aquest apartat documentarem pas a pas la instal·lació del sistema gestor de base de dades mySQL.





![Selecció_604](https://user-images.githubusercontent.com/91249713/173052958-ced5d810-4edc-4cf1-8e8c-2c139c8edc1f.png)


Executant la comanda sudo apt-get install mysql-server instalarem el servidor


![image](https://user-images.githubusercontent.com/91249713/173056306-21f97d99-04e1-4b99-b324-00980826fdc3.png)

- Amb la comanda ps aux | grep mysql podem veure si s'està executant i com s'aprecia a la captura està en execució.

![image](https://user-images.githubusercontent.com/91249713/173056629-0593cd0d-e6ce-47ef-8430-1e4204a2d6e1.png)

- Acte seguit, instalem la eïna nmap, en el meu cas ja la tenia instalada. Per a instalar aquesta eïna executarem la comanda sudo apt-get install nmap, posteriorment farem un escaneig dels port que es troben oberts al localhost i com veem el port 3306 que es el del mysql es troba obert.

![image](https://user-images.githubusercontent.com/91249713/173059253-6a9ceb88-78bf-49fa-917c-20b2fc8e28dc.png)

- Executant la comanda dpkg -L mysql-server-8.0 | grep etc podem veure els fitxers de configuració del paquet mysql-server-8.0.


![image](https://user-images.githubusercontent.com/91249713/173059452-3fac9545-95c8-45b1-afd5-cbd8c52e008d.png)

- Executant dpkg -L mysql-server-8.0 | grep var podem veure les bases de dades.

![image](https://user-images.githubusercontent.com/91249713/173059807-3c92d9b1-11c0-49f8-87c1-4e6624c9d7fc.png)

-Consultant aquest fitxer podrem veure un usuari que crea debian per defecte i sirà amb el que accedirem a mysql.

![image](https://user-images.githubusercontent.com/91249713/173060081-31bb4ef3-c8c1-433e-85bb-5a18e632cda7.png)
- Com podem veure hem accedit correctament a mysql amb aquest usuari.

![image](https://user-images.githubusercontent.com/91249713/173060410-b3cecfec-6543-4b6c-96f6-f881ac518419.png)

- Dins del mysql executant aquesta comanda podrem veure les base de dades creades, aquestes que es mostren a la captura son les pripies del sistema, nosaltres encara no hem creat cap.

![image](https://user-images.githubusercontent.com/91249713/173060585-5b0573a9-903f-4190-b491-7f549fb4afb7.png)
- Amb auqesta altra comanda podrem veure els privilegis.

![image](https://user-images.githubusercontent.com/91249713/173060796-1362a271-7595-4758-90c5-51df9544b28e.png)

- Per a crear una taula introduirem la sentència CREATE DATABASE tasks; i amb el show databases podem veure que ara si que hem creat una nosaltres i ja ens apareix.

![image](https://user-images.githubusercontent.com/91249713/173062218-99542698-c459-466d-9b10-b9f6b2a8647b.png)

- Introduint use tasks; entrarem dins d'aquesta taula que hem creat i una vegada dins crearem les taules. 


![image](https://user-images.githubusercontent.com/91249713/173078009-e1252428-8f18-468a-8d84-6e063739448e.png)

-Instalem el mysql-workbench desde la pàgina web de mysql community downloads i haurem d'instalar-nos els dos ultims paquets que és mostren a la captura.

![image](https://user-images.githubusercontent.com/91249713/173078262-371bc293-d7ec-40c2-bf40-637462ac50f9.png)












