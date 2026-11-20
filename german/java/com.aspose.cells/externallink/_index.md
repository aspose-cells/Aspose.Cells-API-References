---
title: "ExternalLink"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen externen Link in einer Arbeitsmappe dar."
type: docs
url: /de/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Stellt einen externen Link in einer Arbeitsmappe dar.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Fügt einen externen Namen hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Stellt die Datenquelle des externen Links dar. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Stellt die gespeicherte Datenquelle des externen Links dar. |
| [getPathType()](#getPathType--) | Gibt den Pfadtyp dieses externen Links zurück |
| [getType()](#getType--) | Ermittelt den Typ des externen Links. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Gibt an, ob dieser externe Link von anderen referenziert wird. |
| [isVisible()](#isVisible--) | Gibt an, ob dieser externe Link in MS Excel sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Stellt die Datenquelle des externen Links dar. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Stellt die gespeicherte Datenquelle des externen Links dar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Fügt einen externen Namen hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Der Text des externen Namens. Wenn der externe Name zu einem Arbeitsblatt gehört, sollte der Text wie Sheet1!Text sein. |
| referTo | java.lang.String | Der referTo des externen Namens. Es muss eine Zelle oder ein Bereich sein. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


Stellt die Datenquelle des externen Links dar.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Stellt die gespeicherte Datenquelle des externen Links dar.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Gibt den Pfadtyp dieses externen Links zurück

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ des externen Links.

Siehe [ExternalLinkType](../../com.aspose.cells/externallinktype).

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


Gibt an, ob dieser externe Link von anderen referenziert wird.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Gibt an, ob dieser externe Link in MS Excel sichtbar ist.

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


Stellt die Datenquelle des externen Links dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Stellt die gespeicherte Datenquelle des externen Links dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

