---
title: "Hyperlänk"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en hyperlänk."
type: docs
url: /sv/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

Inkapslar objektet som representerar en hyperlänk.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [delete()](#delete--) | Tar bort den här hyperlänken |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Representerar adressen för en hyperlänk. |
| [getArea()](#getArea--) | Hämtar området för hyperlänken. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Hämtar länktypen. |
| [getScreenTip()](#getScreenTip--) | Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken. |
| [getTextToDisplay()](#getTextToDisplay--) | Representerar texten som ska visas för den angivna hyperlänken. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Representerar adressen för en hyperlänk. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Representerar texten som ska visas för den angivna hyperlänken. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


Tar bort den här hyperlänken

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
### getAddress() {#getAddress--}
```
public String getAddress()
```


Representerar adressen för en hyperlänk.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public CellArea getArea()
```


Hämtar området för hyperlänken.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


Hämtar länktypen.

Se [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


Representerar texten som ska visas för den angivna hyperlänken. Standardvärdet är hyperlänkens adress.

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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


Representerar adressen för en hyperlänk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


Representerar texten som ska visas för den angivna hyperlänken. Standardvärdet är hyperlänkens adress.

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

