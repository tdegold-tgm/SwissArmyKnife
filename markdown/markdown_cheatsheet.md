# Markdown Cheatsheet

Eine Übersicht über die gängigsten Mardown-Elemente [[1]](https://support.typora.io/Markdown-Reference).

**Dieses Dokument kann ebenfalls in meinem Repo [[2]]() gefunden werden.**

## Überschriften

Überschriften (1-6) werden über das #-Zeichen definiert.

```
# Überschrift 1
## Überschrift 2
###### Überschrift 6
```

## Zitate

Zitate werden mit dem >-Zeichen definiert. Genestete Zitate sind möglich

```
> Dies ist ein mehrzeiliges Zitat.
> Es erstreckt sich über zwei Zeilen.

> Es ist auch möglich.
> > Genestete Zitate 
> > zu erstellen.
```

## Listen

Ungeordnete Listen können mit den Zeichen +,* und - erstellt werden. Mit 1. usw. können geordnete Listen definiert werden. Es können auch Sublisten erstellt werden. Dabei können geordnete und ungeordnete Losten gemischt werden.

```
## ungeordnete Liste
- Element 1
..- Subelement 1
....- Subsubelement 2

## geordnete Liste
1. Element 1
..1. Subelement 1
```

## Checklisten

```
- [ ] nicht erfüllter Task
- [x] erfüllter Task
```

## Inline Code und Codeblöcke

```
​```
public static void main(String[] args){
	System.out.println("Dies ist ein Codeblock!")
}
​```

​```java
public static void main(String[] args){
	System.out.println("Dies ist ein Codeblock, mit Syntaxhighlighting für Java!")
}
​```
```

```
Die Funktion `test()` wird als Inline Code angezeigt.
```

Die Funktion `test()` wird als Inline Code angezeigt.

## LaTeX

Ein LaTeX-Block kann mit '$$ + Enter' generiert werden

```latex
$$
v = \frac{s}{t}
$$
```

$$
v = \frac{s}{t}
$$

## Fußnoten

```
Fußnoten [^fn1] lassen sich ganz leicht definieren.

[^fn1]: Hier ist sie zu lesen
```

## Links

Der Text in eckigen Klammern wird angezeigt, der Pfad steht in runden Klammern.

```
Dieser [Link](http://example.com/ "Title") hat einen Titel,
dieser [Link](http://example.com/) nicht.
```

Es kann auch innerhalb eines Dokuments referenziert werden.

```
Dazu einfach die [gewünschte Überschrift][#Überschriften] in runden Klammern angeben
```

## Bilder

```
![alt. Text](pfad/zum/bild.png "optionaler Titel")
```

## Hervorhebungen

```
*Dieser Text ist kursiv*
**Dieser Text ist fett gedruckt**
~~Dieser Text ist durchgestrichen~~
```

## HTML

Man kann einfach HTML-Elemente einfügen, um den Text zusätzlich zu designen. z.B.:

```
<span style="color:red">Dieser Text ist rot</span>
```

<span style="color:red">Dieser Text ist rot</span>

## Quellen

**offizielle Website**

[1] "Markdown Reference", typora.io. [Online]. Available: https://support.typora.io/Markdown-Reference. [Accessed: Jan. 27, 2020]



**GitHub Repository**
 [2] T. Degold, "Markdown Cheatsheet", *github.com*. [Online]. Available: https://github.com/tdegold-tgm/SwissArmyKnife/blob/master/Standards_und_Normen/IEEE_zitate.md. [Accessed: Jan. 23, 2020]