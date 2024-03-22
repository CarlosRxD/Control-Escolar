# Control-Escolar
Control Escolar es una plataforma diseñada para facilitar la gestion integral de la información académica y administrativa en instituciones educativas.

Para ejecutar el programa se deben de ejecutar los scripts de la base de datos en MySql
depues en Netbeans 17 en el entorno de java 17 agregamos el proyecto 
ademas de no tener intalado las dependencias de MySql agregaremos en el pom.xml
 <!-- Dependencia para el controlador JDBC de MySQL -->
        <dependency>
            <groupId>mysql</groupId>
            <artifactId>mysql-connector-java</artifactId>
            <version>8.0.33</version> <!-- La versión puede variar -->
            <scope>compile</scope>
        </dependency>
de igual manera para el correcto funcionamiento modificaremos la version del plugin 
<artifactId>maven-war-plugin</artifactId>
de esta manera

            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-war-plugin</artifactId>
                <version>3.3.2</version>
                <configuration>
                    <failOnMissingWebXml>false</failOnMissingWebXml>
                </configuration>
            </plugin>
al terminar de realizar estas modificaciones podremos ejecutar el proyecto ControlEscolar el cual
correra el programa inicial index.jsp el cual mostrara el Inicio del Control Escolar donde el Usuario 
podra registrar, monitorear y analizar datos relacionados con la asistencia, calificaciones 
y datos básicos de los alumnos
Se intenta que el proyecto sea intuitivo para el usuario para el correcto gestionamiento del mismo.
