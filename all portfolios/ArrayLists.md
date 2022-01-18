# Wannabe Quizlet

## Aufgabenstellung
Das Team "Robin" und ich haben mithilfe der Programmiersprache “C#” ein Vocabulary tool Programmiert. Man hat die Möglichkeit mehrere Wörter auf Deutsch und auf Französisch einzuschreiben und anschliessend fragt das Programm den Nutzer ab. 

## Ziele
• Meine Skills mit `ArrayLists` verbesseren.

## Wie benutze ich eine ArrayList?
Um die eingeben Wörter des Nutzers Speichern zu können müssen sie in einem Array eingetragen werden. Also etwa so als würde ich jedes Wort was eingeschrieben wird in einer Kiste packen. Hier ein Beispiel:
```csharp
static void Main(string[] args)
        {
            ArrayList fav_colors = new ArrayList();

            Console.WriteLine("enter your favorite colors:");
            fav_colors.Add(Console.ReadLine());
        }
```
Zuerst haben wir eine Variable mit dem Datentyp `ArrayList` erstellt, also `ArrayList fav_colors = new ArrayList();` 
Danach ganz einfach ein `Console.WriteLine();`, das uns den Inhalt zwischen den Klammern in der Konsole anzeigt, in diesem Fall wird uns in der Konsole also _enter your favortie color:_ angezeigt. Nicht vergessen, reiner Text kommt in den Klammern immer zwischen 2 Gänsefüsschen ("")!. Danach nehmen wir den Namen unserer ArrayList, in diesem fall also `fav_colors` und hängen ein `.Add` an. In den Klammern schreiben wir `Console.ReadLine();` damit der Nutzer etwas eingeben kann in der Konsole. Jetzt haben wir dem Programm gesagt: Alles was ich reinschreibe fügst du zu der `ArrayList fav_colors` zu.   
### Wie können wir nun den Inhalt einer ArrayList auf der Konsole anzeigen?
Dafür machen wir eine Funktion und sagen dem Programm, es soll nach Inhalt in einem bestimmten Array suchen und diesen dann anschliessen drucken. Hier ein Beispiel:
```csharp
public static void PrintValue(IEnumerable myList)
        {
            foreach (Object obj in myList)
                Console.Write($"\n{obj}\n");
        }
```
Zuerst haben wir die Funktion erstellt, also: `public static void PrintValue(IEnumerable myList)`. Innerhalb der Funktion haben wir eine `foreach`- Schleife benutzt. Diese sucht nach Objekten im array `myList`. Sobald er etwas gefunden hat, druckt er den ganzen Inhalt mithilfe von `Console.Write($"{obj}");`. Aber wie können wir nun der Funktion sagen, dass wir den Inhalt unserer Array List wollen? Dafür "Fusionieren" wir beide Code Snippets! Und zwar so:
```csharp
static void Main(string[] args)
        {
            ArrayList fav_colors = new ArrayList();

            Console.WriteLine("enter your favorite colors:");
            fav_colors.Add(Console.ReadLine());
            PrintValue(fav_colors);
        }
        public static void PrintValue(IEnumerable myList)
        {
            foreach (Object obj in myList)
                Console.Write($"\n{obj}\n");
        }
```
Wir haben jetzt beide Code Snippets untereinander aufgeschrieben. Danach haben wir den Namen unserer Funktionen genommen, also `PrintValue` und haben es im oberen Code Snippet mit den Namen unserer `ArrayList` aufgeschrieben, also `PrintValue(fav_colors);`. Nun wird der Inhalt der unserer `ArrayList` gedruckt! Aber wieso? In der Funktion wurde in den Klammern der Datentyp `IEnumerable myList` deklariert. Das bedeutet alles was wir oben in der Klammer von `PrintValue` in den Klammern eingeben haben wird automatisch zur `myList` in der Funktion.
### Beispielvideo:
[![description](https://www.klicksafe.de/fileadmin/_processed_/1/0/csm_Logo_YouTube_01_29755e6f1a.png)](https://youtu.be/Xq0pYuUixdU)
## Reflektion und Verifikation
**Reflektion:**
Die Arbeit lief ganz gut, es gab am Anfang etwas Probleme da wir nicht richtig unsere Arbeit aufgeteilt hatten, jedoch haben wir das in der nächsten LA Stunde schnell gelöst und recht schnell und produktiv gearbeitet.

**Verifikation**
Am Anfang des Projektes hatte ich so gut wie keine Ahnung von ArrayLists jedoch habe ich mithilfe von Igor und Stack Overflow schnell verstanden, wie ArrayLists funktionieren und habe sie dann auch dementsprechend angewendet.
