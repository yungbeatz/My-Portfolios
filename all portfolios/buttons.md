# HatGame

Das Team "🍬" und ich haben mithilfe der Programmiersprache "C#" ein Hütchenspiel programmiert. Man kann mit Startgeld ($300) oder mit dem gewonnenen Geld eine Wette setzten, danach klickt man auf einen der 3 Hüte und mit etwas Glück gewinnt man das gewettete Geld! ^^

## Aufgabenstellung
• Meine Skills mit `buttons` verbesseren.
 

## Wie benutze ich einen `button`?
Da wir ja diesmal auch eine GUI (**G**raphical **U**ser **I**nterface) haben, brauchen wir auch dementsprechend auch die sogenannten `buttons`, um unser Spiel umso besser zu machen! Im `Windows Forms` müssen wir diese `buttons` zweimal in unser Programm implementieren: Einmal ziehen wir einen `button` aus der `Toolbox` (eine Liste mit allen möglichen Tools, die man in einem GUI mit Windows Forms benutzen kann) in unser `Form.cs [Design]` (also das Default Interface von unserem Programm) und gleichzeitig wird automatisch eine `funktion` im `Program.cs` (der ganze Source Code unseres Programmes) generiert zu diesem `button` den wir erst gerade in unsere `Form.cs [Design]` eingefügt haben.
Hier ein beispiel:
Unser `button` im `Program.cs`
```csharp
private void button1_Click(object sender, EventArgs e)
        {

        }
        
```
Unser `button` im `Form.cs [Design]`



[![description](https://media.giphy.com/media/bTRqUfkXtaBIj9PkQf/giphy.gif)](https://media.giphy.com/media/bTRqUfkXtaBIj9PkQf/giphy.gif)



*(If the gif is too small, click on it to see a resized version of it.)*
  
## Wie machen wir jetzt so ein button nützlich? 
 Das ist eigentlich ganz einfach! Es gibt 2 Sachen, die wir mit diesem `button` machen können: 
• Den `button` eine Funktion geben.
• Den `button` visuell verändern.
 
 ####  Den button visuell verändern:
 Nun befinden wir uns im `Form.cs [Desgin]` und haben unseren `button` ausgewählt, sehen wir rechts unten einen Tab mit allen Eigenschaften des `buttons`. Dort können wir die Farbe, die Schriftgrösse, die Schriftart und vieles mehr ändern!



 Hier ein Bild dazu:



 [![description](https://i.ibb.co/v3G5rDX/Screenshot-2021-12-21-144834.jpg)](https://i.ibb.co/v3G5rDX/Screenshot-2021-12-21-144834.jpg)



 *(If the image is too small, click on it to see a resized version of it.)*


 #### Dem button eine Funktion geben:
Natürlich können wir auch die Funktion des `buttons` verändern in dem wir in der Auto-generierten `function` unseren Code für den `button` schreiben. Hier ein Beispiel:
```csharp
        private void button1_Click(object sender, EventArgs e)
        {
            MessageBox.Show("Ich bin ein Pop-Up");
        }
```
Hier haben wir nun `MessageBox.Show("Ich bin ein Pop-Up");` hinzugefügt! Wenn wir nun auf den `button` klicken wird eine `MessageBox` (Ein kleines Fenster) mit dem Text *"Ich bin ein Pop-Up"* geöffnet!



Hier ein visuelles Beispiel:



[![description](https://media.giphy.com/media/cEio37xIvAsQFFmLfH/giphy.gif)](https://media.giphy.com/media/cEio37xIvAsQFFmLfH/giphy.gif)



 *(If the gif is too small, click on it to see a resized version of it.)*

## Reflektion und Verifikation



**Reflektion:**



In der Gruppe habe ich diesmal zu den "schwächeren" gehört, ich habe recht viele an hiebe gebraucht bis ich etwa den dreh raus hatte effektiv mit `Windows Forms` zu arbeiten, zum Beispiel habe ich etwa 40 Minuten gebraucht bis ich es geschafft hatte den Wert eines `Integers` in einem `Label` anzeigen zu können, sobald das Programm lief. 



**Verifikation**



Mithilfe von Vin und Ilona habe ich schnell gelernt, wie ich `buttons` richtig und effektiv nutze! Ich habe definitiv meine Skills mit `buttons` verbessert!
Fürs nächste mal möchte ich mich mehr ins zeug legen wenn wir wieder mit Windows Forms arbeiten damit ich dann auch viel zum Projekt beitragen kann.
