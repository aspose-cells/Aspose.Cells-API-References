---
title: "ExternalLink"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en extern länk i en arbetsbok."
type: docs
url: /sv/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Representerar en extern länk i en arbetsbok.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Lägger till ett externt namn. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Representerar datakälla för den externa länken. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Representerar lagrad datakälla för den externa länken. |
| [getPathType()](#getPathType--) | Hämta sökvägstypen för denna externa länk |
| [getType()](#getType--) | Hämtar typen av extern länk. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Anger om denna externa länk refereras av andra. |
| [isVisible()](#isVisible--) | Anger om denna externa länk är synlig i MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Representerar datakälla för den externa länken. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Representerar lagrad datakälla för den externa länken. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Lägger till ett externt namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten för det externa namnet. Om det externa namnet tillhör ett kalkylblad ska texten vara som Sheet1!Text. |
| referTo | java.lang.String | Referensen (referTo) för det externa namnet. Det måste vara en cell eller ett område. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


Representerar datakälla för den externa länken.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Representerar lagrad datakälla för den externa länken.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Hämta sökvägstypen för denna externa länk

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av extern länk.

Se [ExternalLinkType](../../com.aspose.cells/externallinktype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Anger om denna externa länk refereras av andra.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Anger om denna externa länk är synlig i MS Excel.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


Representerar datakälla för den externa länken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Representerar lagrad datakälla för den externa länken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

