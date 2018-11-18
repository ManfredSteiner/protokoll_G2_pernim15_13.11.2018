# 2. Protokoll

![](https://www.htl-kaindorf.at/images/startpage/logoMecha.png) 

Name: Perl Nicolas  
Kat.-Nr.: 10  
Klasse: 4AHME  
Gruppe: 2  

| Anwesend | Abwesend |  
| --------------------------------------- | -------- |  
| M.Korrenn, A.Murko, D.Orthofer, N.Perl, S.Szapacs | J.Skof |  
___

### Themen-Übersicht
 - **1)** - Die Kompilierung
	 - 1.1) - *Grundbegriffe der Kompilierung* 
 - **2)** - Wichtige Bash-Commands  
 - **3)** - Manuelles Kompilieren mithilfe der Konsole
 
 ___
	  
## 1) Die Kompilierung

![](http://www.ntu.edu.sg/home/ehchua/programming/cpp/images/C_DevelopmentProcesses.png)

Quelle: [The Process of Writing a C Program](http://www.ntu.edu.sg/home/ehchua/programming/cpp/c0_Introduction.html)  

___

### 1.1) - *Grundbegriffe der Kompilierung* 

**- Was ist ein Präprozessor? -**  
Ein Präprozessor ist ein eigenständiges Computerprogramm, das durch den Compiler als erster Schritt der Übersetzung aufgerufen wird. Er löst Präprozessorbefehle in der Quelldatei auf und ersetzt diese durch die jeweilige Funktionalität. Präprozessorbefehle sind am davorliegenden **#** erkennbar.

**- Was ist ein Compiler? -**  
Ein **Compiler** ist ein Programm, das in einer höheren Programmiersprache wie z.B. C verfassten Quellcode in maschinenlesbare Sprache (Assemblersprache) übersetzt. 

**- Wie arbeitet ein Compiler? -**  
Ein **Compiler** arbeitet sich immer komplett durch ein gesamtes Dokument durch. Auf diese Weise unterscheidet sich seine Arbeit vom  Interpreter. Bevor der Compiler höheren Quellcode in maschinenlesbare Zielsprache übersetzen kann, muss der Quellcode gescannt und Programmsymbole extrahiert werden. 
Wichtig ist, dass der Compiler trotz Fehler im Code weiterarbeitet. Ansonsten kann der Quellcode nicht in maschinenlesbare Zielsprachen übertragen werden.

**- Was ist ein Assembler? -**  
Der **Assembler** ist eine Programmiersprache, welche eine für Menschen bessere, lesbare Repräsentation der Maschinensprache ist. Als _Assembler_ wird nicht nur die Sprache selbst, sondern auch ihr Compile benannt. Übersetzt der Compiler ein Assembler-Programm in die Maschinensprache, so nennt man den Vorgang "_assemblieren_". Den umgekehrten Vorgang nennt man "_disassemblieren_".

**- Was ist ein Linker? -**  
Ein **Linker** hilft dem Programmierer, die übersetzten Programme zum Ablauf zu bringen. Die kompilierten Objektprogramme sind noch nicht lauffähig. Da im Quellprogramm verlangte Programmteile, wie z.B. Ein- und Ausgabeprozeduren, hinzugefügt werden müssen, bindet der Linker diesen Objektcode mit externen Bibliotheken zusammen. Produkt dieses Prozesses ist dann das ausführbare Programm.

**- Was ist ein GCC-Compiler -**  
Der C-Compiler von **GNU**, *_gcc_*, ist einer der vielseitigsten und fortschrittlichsten aller verfügbaren Compiler. Anders als andere C-Compiler unterstützt _gcc_ alle modernen C-Standards - etwa ANSI-C - sowie viele Erweiterungen, die nur in _gcc_ zu finden sind. 

![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/GCC_Schema.svg/600px-GCC_Schema.svg.png)

**- Was ist ein Terminal/Shell/Bash? -**
Weil die direkte Kommunikation mit dem Betriebssystem-Kern für einen Benutzer viel zu komplex wäre, ist eine vereinfachte Benutzer-Schnittstelle erforderlich. Neben einer grafischen Schnittstelle wie dem X Window System wird diese Leistung vor allem von einer Shell bereitgestellt. Der englische Ausdruck **Shell**, zu Deutsch etwa **Schale** oder **Ummantelung**, drückt diesen Sachverhalt bereits aus. Die Übersetzung oder Symbolisierung als **Muschel** hat dabei wohl mehr mit Spieltrieb und Anschaulichkeit als mit einem echten technischen Hintergrund zu tun. Jedenfalls lässt sich eine Shell als eine Schicht zwischen Betriebssystem und Benutzer verstehen.

Während Benutzer, die noch nicht häufig mit Shells in Berührung gekommen sind, den wartenden Eingabeprompt einer Shell als trist und abweisend, ja sogar als Hindernis empfinden mögen, wurden Shells doch mit der gegenteiligen Absicht entwickelt: Sie sollten die tägliche Arbeit vereinfachen und erleichtern.

**- Was ist eine Bibliothek? -**
Bibliotheken Die C-Standard-Bibliothek (englisch C standard library) ist die Standardbibliothek der Programmiersprache C. In jeder standardkonformen betriebssystemgestützten Implementierung (hosted environment) von C muss die C-Standard-Bibliothek in vollem Umfang vorhanden sein. Hingegen müssen freistehende Umgebungen (freestanding environment), wie man sie beispielsweise im Embedded-Bereich häufig antrifft, nur eine festgelegte Untermenge der Standardbibliothek anbieten, um standardkonform zu sein.

___

## 2) Wichtige Bash-Commands

| Befehl | Funktion |  
| ------ | -------- |  
| `pwd` | Gibt das Verzeichnis aus |  
| `whoami`| Welches Nutzerprofil nutze ich |  
| `cd` | Verzeichnisbaum ändern |
| `/` | etwas bestimmtes Suchen |
| `ls` | um alle Hauptverzeichnisse anzuzeigen, die unter einem bestimmten Dateisystem abgelegt sind. |
| `man` | um das Handbuch des eingegebenen Begriffes anzuzeigen |  
| `G` | Nach ganz oben gelangen |  
| `g` | Nach ganz unten gelangen |
| `n` | next |  
| `h` | mehr |  
| `q` | quit |  
| `echo` | Nachricht auf dem Bildschirm anzeigen |  
| `which` | Durchsuchen Sie den $ Pfad des Benutzers nach einer Programmdatei |  
| `type` | Was für eine Art ist ein Command |  
| `mkdir` | Verzeichnis erstellen |  
| `mv` | über sehr weite Pfade Verzeichnisse verscheieben |  
| `cp` | kopieren (nur von Dateien) |  
| `alias` | best. Commandoabkürzungen selbst definieren |  
| `rm` | Dateien löschen |  
| `rmdir` | löscht (nur!) leere Verzeichnisse |  
| `rm -r` | löscht Dateien oder Verzeichnisse egal ob beschrieben |  
| `touch` | ändert den Zeitstempel der Datei |  
| `history` | Command History anzeigen |  
| `nano ~/.bash_history` | history ist hier gespeichert |  
| `!(Zahl des Commands)` | um spezielles Command wiederaufzurufen |  
| `rsync -aP ue01/* ue02/` | remote synchronise = alles kopieren von ue01 mit Progress-Bar in ue02
| `find` | Suchen von Dateien |  
| `nano` | öffnen des Linux Command-Line Text Editors |  
| `cat` | Verkettet den Inhalt von Dateien und zeigt ihn an |  
| `less` | Zeigt Sie die Ausgabe für einen Bildschirm an |  

[A-Z Index of the Linux command lines](https://ss64.com/bash/)

___

## 3) Manuelles Kompilieren mithilfe der Konsole

`nano main.c` 
```
#incude <stdio.h>
int main()
{
printf("Hallo, Guten Morgen\n");
return 0;
}
```

Strg + o Datei wird gespeichert
Strg + x Editor wird beendet

**Kompilierungsvorgang:**  

 `gcc **-E** main.c `    | - Präprozessieren zum Preprozessorquelltext  
 `gcc **-S** main.c `    | - Kompilieren zum Assemblerquelltext  
 `gcc **-c** main.c `    | - Assemblieren zur Objektdatei (object datei)  
 `hexdump -C ("main.c")`    | - Anzeigen des Codes auf der Konsole in Hexadezimal  
 `gcc **-o** main.c `    | - Object Datei erstellen  

 ![](https://bvinothraj.files.wordpress.com/2010/01/compile.jpg)  
 
