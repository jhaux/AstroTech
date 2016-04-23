# README #

### What is this repository for? ###

repo for Astronomical Techniques

File structure
Wenn das für Euch in Ordnung ist, würde ich folgende Ordnerstruktur vorschlagen:
fundamentals/
> zettelX/
>
>> Makefile # nutzt den Ordernamen als Variable
>> 
>>> Regeln: make, make docu, make clean
>>
>> bin/ # hier werden die executables hingepackt wenn "make" ausgeführt wird
>>
>> src/ # hier kommt unser sourcecode hin
>>
>>> zettelX.c # Das ist die main Datei, sie muss wie der Ordner heissen
>>
>> doc/ # hier kommt die .tex datei für die Abgabe hin
>>
>>> zettelX.tex # die Datei muss wie der Ordner heissen
>>
>> pic/ # ggf. für Bilder, die wir in unser tex dokument einpflegen wollen

Das script `zettel` kann man per `./zettel int` ausführen, wobei `int` für die 
aktuelle Zettelnummer steht. Das Skript ist sehr einfach gehalten, es können 
Fehler passieren :)
Sinn ist es, einfach die Ordnerstruktur zu bauen (s.o.) und das alte `.tex` 
Dokument und den `Makefile`, falls vorhanden zu kopieren. 

Der `Makefile` muss noch getestet werden.
