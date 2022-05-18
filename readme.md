Projeto para gerar entidades a partir de bancos de dados

para rodar voce deve mudar as propriedades do arquivo hibernate.properties
com os valores para conectar no seu banco de dados:
hibernate.connection.driver_class=org.postgresql.Driver
hibernate.connection.url=jdbc:postgresql://localhost:5432/postgres
hibernate.connection.username=cadastro
hibernate.connection.password=cadastro
hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

a linha de comando deve ser:
va até a raiz do projeto:
cd generateEntity
e depois execute:
mvn hibernate3:hbm2java

as entidades serão geradas no diretorio:
src/main/java

por exemplo:

com.blog.hbm.pojo
/generateEntity/src/main/java/com/blog/hbm/pojo/FlywaySchemaHistory.java
/generateEntity/src/main/java/com/blog/hbm/pojo/Localizacao.java
/generateEntity/src/main/java/com/blog/hbm/pojo/Prato.java
/generateEntity/src/main/java/com/blog/hbm/pojo/Restaurante.java