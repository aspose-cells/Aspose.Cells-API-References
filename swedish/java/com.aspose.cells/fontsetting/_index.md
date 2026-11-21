---
title: "FontSetting"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett intervall av tecken inom celltexten."
type: docs
url: /sv/java/com.aspose.cells/fontsetting/
---

**Inheritance:**
java.lang.Object
```
public class FontSetting
```

Representerar ett intervall av tecken inom celltexten.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         //getting characters
         FontSetting character = cell.characters(6, 7);
 
         //Setting the font of selected characters to bold
         character.getFont().setBold(true);
 
         //Setting the font color of selected characters to blue
         character.getFont().setColor(Color.getBlue());
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [FontSetting(int startIndex, int length, WorksheetCollection sheets)](#FontSetting-int-int-com.aspose.cells.WorksheetCollection-) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Returnerar teckensnittet för detta objekt. |
| [getLength()](#getLength--) | Hämtar längden på tecknen. |
| [getStartIndex()](#getStartIndex--) | Hämtar startindexet för tecknen. |
| [getTextOptions()](#getTextOptions--) | Returnerar textalternativen. |
| [getType()](#getType--) | Hämtar typen av textnod. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Ställer in den förinställda WordArt-stilen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontSetting(int startIndex, int length, WorksheetCollection sheets) {#FontSetting-int-int-com.aspose.cells.WorksheetCollection-}
```
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int |  |
| length | int |  |
| sheets | [WorksheetCollection](../../com.aspose.cells/worksheetcollection) |  |

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
### getFont() {#getFont--}
```
public Font getFont()
```


Returnerar teckensnittet för detta objekt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Hämtar längden på tecknen.

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Hämtar startindexet för tecknen.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Returnerar textalternativen.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av textnod.

Se [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
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




### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Ställer in den förinställda WordArt-stilen.

**Remarks**

Endast för texten i form/diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Den förinställda WordArt-stilen. |

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

