# Tutorial_AllureReportDemo_Java_TestNg


Primero cree el proyecto maven como de costumbre 

configuro el pom 
busca cada dependencia en el maven repository
https://mvnrepository.com/artifact/io.qameta.allure/allure-testng/2.21.0
Ejemplo
	  <!-- https://mvnrepository.com/artifact/org.testng/testng -->
	<dependency>
	    <groupId>org.testng</groupId>
	    <artifactId>testng</artifactId>
	    <version>7.7.1</version>
	    <scope>test</scope>
	</dependency>
	
	<!-- https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java -->
	<dependency>
	    <groupId>org.seleniumhq.selenium</groupId>
	    <artifactId>selenium-java</artifactId>
	    <version>4.8.3</version>
	</dependency>
	
	<!-- https://mvnrepository.com/artifact/io.github.bonigarcia/webdrivermanager -->
	<dependency>
	    <groupId>io.github.bonigarcia</groupId>
	    <artifactId>webdrivermanager</artifactId>
	    <version>5.3.2</version>
	</dependency>

<!-- https://mvnrepository.com/artifact/io.qameta.allure/allure-testng -->
	<dependency>
	    <groupId>io.qameta.allure</groupId>
	    <artifactId>allure-testng</artifactId>
	    <version>2.21.0</version>
	</dependency>
	
	
click derecho al proyecto maven -> Update Proyect	
	
luego en src/test/java 
crea el paquete 
al paquete click derecho crear new other testng(en market place busque el TestNg y lo instale al plugin porque no aparecia) y le puse el nombre al nombre de esa clase testcase1.java
copie y pegue y se creo el otro testcase2.java

click derecho en cada uno y lo puedo correr aparte 
con run as TestNg

luego click derecho en el package TestNG -> Convert To TestNG
cambio el nombre de la Suite 
por ejemplo SmokeTesting y finish 
ahora aparece al mismo nivel el testng.xml
click derecho ahi dentro del file  testng.xml run as TestNG
y me deberia correr los test en consola 

ahora el tipo instalo allure y mvn 

luego click derecho al proyecto maven update 


me voy a la ubicacion del proyecto abro una terminal y escribo 
allure serve
y  abre el reporte en el browser