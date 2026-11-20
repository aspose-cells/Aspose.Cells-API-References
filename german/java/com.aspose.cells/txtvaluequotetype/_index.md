---
title: "TxtValueQuoteType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt den Typ der Verwendung von Anführungszeichen für Werte in Textformatdateien an."
type: docs
url: /de/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

Gibt den Typ der Verwendung von Anführungszeichen für Werte in Textformatdateien an.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ALWAYS](#ALWAYS) | Alle Werte werden immer in Anführungszeichen gesetzt. |
| [MINIMUM](#MINIMUM) | Werte nur bei Bedarf in Anführungszeichen setzen. |
| [NEVER](#NEVER) | Alle Werte werden nicht in Anführungszeichen gesetzt. |
| [NORMAL](#NORMAL) | Alle Werte, die Sonderzeichen wie Anführungszeichen oder Trennzeichen enthalten, werden in Anführungszeichen gesetzt. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Alle Werte werden immer in Anführungszeichen gesetzt.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


Werte nur bei Bedarf in Anführungszeichen setzen. Zum Beispiel, wenn ein Wert ein Anführungszeichen enthält, das jedoch nicht am Anfang dieses Wertes steht, wird dieser Wert nicht in Anführungszeichen gesetzt.

### NEVER {#NEVER}
```
public static final int NEVER
```


Alle Werte werden nicht in Anführungszeichen gesetzt. Die exportierte Textdatei dieses Typs kann möglicherweise nicht korrekt wieder eingelesen werden, weil die erforderlichen Anführungszeichen fehlen.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Alle Werte, die Sonderzeichen wie Anführungszeichen oder Trennzeichen enthalten, werden in Anführungszeichen gesetzt. Entspricht dem Verhalten von MS Excel beim Exportieren von Textdateien.

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

