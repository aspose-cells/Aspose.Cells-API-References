---
title: "SpreadsheetSplitter"
second_title: "Aspose.Cells för Java API-referens"
description: "Delar upp kalkylbladsfilen i flera delar."
type: docs
url: /sv/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

Delar upp kalkylbladsfilen i flera delar.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | Delar upp kalkylbladsfilen i flera delar. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Delar den angivna mallfilen i flera delar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Delar upp kalkylbladsfilen i flera delar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | Alternativ för att dela kalkylblad |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Delar den angivna mallfilen i flera delar.

**Remarks**

Utdatafilerna kommer att byggas från den angivna resulterande filen genom att lägga till sekvensnumret för bladet och delningsdelen. Till exempel, om den angivna utdatafilen är Split.xlsx, kommer de genererade filerna att vara Split\_0\_0.xlsx, Split\_0\_1.xlsx, ..., Split\_1\_0.xlsx, ...

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | java.lang.String | Mallfilen som ska delas |
| resultFile | java.lang.String | Den resulterande filen (namnmönster) |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

