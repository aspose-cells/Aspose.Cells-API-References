---
title: "SpreadsheetSplitter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Teilt Tabellendatei in mehrere Teile."
type: docs
url: /de/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

Teilt Tabellendatei in mehrere Teile.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | Teilt Tabellendatei in mehrere Teile. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Teilt die angegebene Vorlagendatei in mehrere Teile. |
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




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


Teilt Tabellendatei in mehrere Teile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | Optionen zum Aufteilen der Tabellenkalkulation |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Teilt die angegebene Vorlagendatei in mehrere Teile.

**Remarks**

Die Ausgabedateien werden aus der angegebenen Ergebnisdatei erstellt, indem die laufende Nummer des Blatts und des geteilten Teils angehängt wird. Zum Beispiel, wenn die angegebene Ausgabedatei Split.xlsx ist, dann werden die erzeugten Dateien Split\_0\_0.xlsx, Split\_0\_1.xlsx, ..., Split\_1\_0.xlsx, ...

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | java.lang.String | Die zu teilende Vorlagendatei |
| resultFile | java.lang.String | Die Ergebnisdatei (Namensmuster) |

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

