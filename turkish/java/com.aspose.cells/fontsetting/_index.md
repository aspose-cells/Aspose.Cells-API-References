---
title: "FontSetting"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre metni içindeki bir karakter aralığını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/fontsetting/
---

**Inheritance:**
java.lang.Object
```
public class FontSetting
```

Hücre metni içindeki bir karakter aralığını temsil eder.

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
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FontSetting(int startIndex, int length, WorksheetCollection sheets)](#FontSetting-int-int-com.aspose.cells.WorksheetCollection-) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Bu nesnenin yazı tipini döndürür. |
| [getLength()](#getLength--) | Karakterlerin uzunluğunu alır. |
| [getStartIndex()](#getStartIndex--) | Karakterlerin başlangıç indeksini alır. |
| [getTextOptions()](#getTextOptions--) | Metin seçeneklerini döndürür. |
| [getType()](#getType--) | Metin düğümünün tipini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Önceden ayarlanmış WordArt stilini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontSetting(int startIndex, int length, WorksheetCollection sheets) {#FontSetting-int-int-com.aspose.cells.WorksheetCollection-}
```
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int |  |
| length | int |  |
| sheets | [WorksheetCollection](../../com.aspose.cells/worksheetcollection) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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


Bu nesnenin yazı tipini döndürür.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Karakterlerin uzunluğunu alır.

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Karakterlerin başlangıç indeksini alır.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Metin seçeneklerini döndürür.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Metin düğümünün tipini alır.

Bkz. [TextNodeType](../../com.aspose.cells/textnodetype).

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


Önceden ayarlanmış WordArt stilini ayarlar.

**Remarks**

Yalnızca şekil/grafik metni için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Önceden ayarlanmış WordArt stili. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

