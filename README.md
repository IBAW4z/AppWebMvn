# AppWebMvn
przykład z wykładu 7 - AplikacjaWebowa przy pomocy Maven (bez tomcata)

instrukcja przyklad7-mvn:
1. Instalacja i konfiguracja mvn: http://www.avajava.com/tutorials/lessons/what-is-maven-and-how-do-i-install-it.html
2. Otwieramy Command Window (Start-->uruchom-->cmd)
3. przechodzimy do katalogu gdzie ma byc zapisana aplikacja (instrukcja cd działa)
4. wpisujemy polecenie: mvn archetype:generate-DgroupId={project-packaging} -DartifactId={project-name} -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false
5. otwieramy powstały projekt w eclipse/intelliJ
6. dodajemy folder "java" w folderze "src/main"
7. w folderze java tworzymy plik "HelloWorld.java":
8. edytujemy plik web.xml (w folderze src/webapp/web-inf):
9. edytujemy plik pom.xml
10. w cmd wpisujemy: mvn compile
potem: mvn package
(gdzies w ciagu znaczkow powinno byc BUILD SUCCES) --> pierwsze uruchamianie bedzie dlugie bo sciaga sobie wszystkie pluginy i to co mu potrzebne (nie wiem jak to sie ma do transferu jesli ktos ma limitowany Internet ;/)
11. wpisujemy w cmd: mvn jetty:run -Djetty.port=8888 (lub jakis inny numer, ale nie 8080 bo to blokuje Labview na pewno)
12. wpisujemy w przegladarce inetrenetowej: localhost:8888/HelloWorld
13. Ogladamy napis Hello World! w przeglądarce i jesteśmy z siebie dumni (nie zastanawiając się, że wyświetlenie głupiego napisu zajeło nam pół dnia ;)
