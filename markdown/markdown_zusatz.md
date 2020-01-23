# Markdown Ergänzungen

von Tim Degold, begonnen am 18.09.2019

## Markdown

Alle grundsätzlichen Funktionen von Markdown können im [Cheatsheet](https://devhints.io/markdown) nachgelesen werden. 

## In einem Dokument referenzieren

mit `<a name="blabla"></a>` kann ein Element benannt werden und mittels `[dieser Text wird plain angezeigt](#blabla)` referenziert werden.

## Bilder in GITHUB

In github werden die Bilder nur angezeigt wenn sie in der Form

```bash
![alt_text](img/bild.ext)
```

angegeben werden. 

## Seitenumbruch in Markdown

Um in Markdown einen Seitenumbruch einzubinden (wenn zum Beispiel in ein PDF exportiert werden soll und jedes Kapitel auf einer neuen Seite beginnen muss) kann das mit folgendem Code getan werden.

```bash
<div style="page-break-after: always;"></div>
```

Diesen einfach im Dokument (**außerhalb eines Code-Blocks**) einfügen.