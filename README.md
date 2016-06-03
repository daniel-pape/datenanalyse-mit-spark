# Datenanalyse mit Spark und Apache Zeppelin

Dieses Repository enthält den Quellcode zum Artikel "Datenanalyse mit Spark und Apache Zeppelin" im Java Magazin 07/2016.

Der Quellcode liegt in Form von Zeppelin-Notebooks im Verzeichnis [notebooks](notebooks).

Mit Docker kann man lokal Zeppelin inklusive Spark leicht starten und ausprobieren. Das Docker Image `aquila/zeppelin` ist für den Einstieg am besten geeignet. Zum Start einfach
```
docker run -p 8080:8080 aquila/zeppelin
```
in einer geeigneten Kommandozeile (z.B. im *Docker Quick Start Terminal*) ausführen. Anschließend ist Zeppelin unter [http://localhost:8080](http://localhost:8080) im Browser erreichbar. Bei der Verwendung von `docker-machine` oder `boot2docker` muss statt `localhost` die IP-Adresse der Docker-VM verwendet werden.

In der Zeppelin-UI können Notebooks mit **Import Notebook** hochgeladen werden. Das wichtigste und interessanteste Notebook ist [Datenanalyse-mit-Spark.json](notebooks/Datenanalyse-mit-Spark.json). Alle weiteren Schritte (z.B. Download der Demodaten) sind im Notebook erklärt.
