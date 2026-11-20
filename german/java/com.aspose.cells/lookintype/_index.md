---
title: "LookInType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Typ für Look‑In dar."
type: docs
url: /de/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

Stellt den Typ für Look‑In dar.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [COMMENTS](#COMMENTS) | Findet das Objekt nur aus dem Kommentar der Zelle. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Findet das Objekt nur aus dem formatierten Wert der Zelle([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [FORMULAS](#FORMULAS) | Findet das gesuchte Objekt aus der Formel([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)), wenn die Zelle eine Formel ist, andernfalls aus dem Originalwert der Zelle (wie bei [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Ignoriert Zellen, die keine Formel sind. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Findet das Objekt nur aus dem Originalwert der Zelle. |
| [VALUES](#VALUES) | Findet das Objekt aus dem Originalwert der Zelle([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) und dem formatierten Wert([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Ignoriert Zellen, die eine Formel sind. |
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
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Findet das Objekt nur aus dem Kommentar der Zelle. Ignoriert Zellen, die keinen Kommentar haben.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Findet das Objekt nur aus dem formatierten Wert der Zelle([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Findet das gesuchte Objekt aus der Formel([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)), wenn die Zelle eine Formel ist, andernfalls aus dem Originalwert der Zelle (wie bei [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Ignoriert Zellen, die keine Formel sind. Für Zellen, die eine Formel sind, wird das gesuchte Objekt aus der Formel([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) gefunden.

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Findet das Objekt nur aus dem Originalwert der Zelle.

### VALUES {#VALUES}
```
public static final int VALUES
```


Findet das Objekt aus dem Originalwert der Zelle([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) und dem formatierten Wert([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Ignoriert Zellen, die eine Formel sind. Für Zellen, die keine Formel sind, entspricht es dem [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

