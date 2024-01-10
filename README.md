# Tasca S4.01 Introducció a Spring - Nivell 1

Exercici Spring i Maven

Aquest exercici és un primer contacte amb Spring i Maven.

Accedeix a la pàgina ->https://start.spring.io/, i genera un projecte Spring boot amb les següents característiques:

- PROJECT (gestor de dependències): Maven

- LANGUAGE: Java.

- SPRING BOOT: La darrera versió estable.

- PROJECT METADATA

  - Group: cat.itacademy.barcelonactiva.cognoms.nom.s04.t01.n01

  - Artifact: S04T01N01GognomsNom

  - Name: S04T01N01GognomsNom

  - Description: S04T01N01GognomsNom

  - Package name: cat.itacademy.barcelonactiva.cognoms.nom.s04.t01.n01

- PACKAGING: Jar

- JAVA: Mínim versió 11 

- Dependències:

  - Spring Boot DevTools

  - Spring Web


Importa’l a Eclipse amb l’opció File > Import > Existing Maven Project.

A l’arxiu application.properties, configura la variable server.port amb el valor 9000.

Convertirem aquesta aplicació en una API REST:

Depenent del package principal, crea un altre subpackage anomenat Controllers, i dins seu, afegeix la classe HelloWorldController.

Haurà de tenir dos mètodes:
    String saluda
    String saluda2

Aquests dos mètodes rebran un paràmetre String anomenat nom, i retornaran la frase:

“Hola, “ + nom + “. Estàs executant un projecte Maven”.


El primer mètode respondrà a una petició GET, i haurà de ser configurat per a rebre el paràmetre com un RequestParam. El paràmetre "nom" tindrà el valor per defecte “UNKNOWN”.

Haurà de respondre a:

    http://localhost:9000/HelloWorld
    http://localhost:9000/HelloWorld?nom=El meu nom

El segon mètode respondrà a una petició GET, i haurà de ser configurat per a rebre el paràmetre com una PathVariable. El paràmetre "nom" serà opcional.

Haurà de respondre a:

    http://localhost:9000/HelloWorld2
    http://localhost:9000/HelloWorld2/el meu nom

## Recursos adicionales
StackOverflow - Service layer: https://stackoverflow.com/questions/5702391/mvcs-model-view-controller-service
Youtube - Julian Mesa - Postman: https://www.youtube.com/playlist?list=PLeo6Q1inqlOeC_zQMg2i3aZcGF_Jmyqd4
