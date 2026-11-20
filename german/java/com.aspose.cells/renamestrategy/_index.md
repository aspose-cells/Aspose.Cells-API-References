---
title: "RenameStrategy"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Strategieoption für doppelte Spaltennamen."
type: docs
url: /de/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Strategieoption für doppelte Spaltennamen.

**Remarks**

Beim Verarbeiten von Daten mit Kopfzeilen erfordern einige Szenarien, dass die Kopfzeilen für alle Spalten nicht dupliziert werden. Zum Beispiel, wenn Daten in eine Datentabelle exportiert werden und die Kopfzeile als Spaltenname der Datentabelle verwendet werden soll, sind duplizierte Werte der Kopfzeile ungültig. Für solche Situationen kann der Benutzer bestimmen, wie sie zu behandeln sind, indem er diese Strategie angibt.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [DIGIT](#DIGIT) | Benannt mit Ziffer. |
| [EXCEPTION](#EXCEPTION) | Wirft Ausnahme. |
| [LETTER](#LETTER) | Benannt mit Buchstabe.. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Benannt mit Ziffer. Duplizierte Namen werden zu ...1, ...2, usw.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


Wirft Ausnahme.

### LETTER {#LETTER}
```
public static final int LETTER
```


Benannt mit Buchstabe.. Duplizierte Namen werden zu ...A, ...B, usw.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

