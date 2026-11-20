---
title: "SplitPartInfo"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Informationen eines Eingabe-/Ausgabe-Elements für mehrere Eingaben/Ausgaben dar, z. B. die aktuelle Seite, die beim Konvertieren einer Tabelle in ein Bild gerendert wird."
type: docs
url: /de/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Stellt die Informationen eines Eingabe-/Ausgabe-Paares für mehrere Eingaben/Ausgaben dar, z. B. die aktuelle Seite, die beim Konvertieren einer Tabelle in ein Bild gerendert wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Index des aktuellen Teils in der Sequenz (0‑basiert). |
| [getSheetIndex()](#getSheetIndex--) | Index des Blatts, in dem sich der aktuelle Teil befindet. -1 bedeutet, dass es nur ein Blatt gibt. |
| [getSheetName()](#getSheetName--) | Name des Blatts, in dem sich der aktuelle Teil befindet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Index des aktuellen Teils in der Sequenz (0‑basiert). -1 bedeutet, dass es keine mehreren Teile gibt, sodass das Ergebnis einzeln ist.

**Remarks**

Wenn mehrere Tabellen verarbeitet werden müssen und jede Tabelle separat (aufgeteilt) verarbeitet wird, beginnt der Teil‑Index für jede Tabelle immer bei 0. Zum Beispiel, beim Konvertieren einer Arbeitsmappe in Bilder, stellt er den Ausgabeseiten‑Index des aktuell verarbeiteten Tabellenblatts dar. Und -1 bedeutet, dass es nur eine Seite für das aktuelle Tabellenblatt gibt.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Index des Blatts, in dem sich der aktuelle Teil befindet. -1 bedeutet, dass es nur ein Blatt gibt.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Name des Blatts, in dem sich der aktuelle Teil befindet.

**Remarks**

Kann in einigen Situationen null sein, zum Beispiel beim Rendern der gesamten Arbeitsmappe zu einem TIFF‑Bild.

**Returns:**
java.lang.String
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

