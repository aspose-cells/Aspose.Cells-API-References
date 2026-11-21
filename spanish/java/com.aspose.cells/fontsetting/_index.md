---
title: "FontSetting"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un rango de caracteres dentro del texto de la celda."
type: docs
url: /es/java/com.aspose.cells/fontsetting/
---

**Inheritance:**
java.lang.Object
```
public class FontSetting
```

Representa un rango de caracteres dentro del texto de la celda.

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
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FontSetting(int startIndex, int length, WorksheetCollection sheets)](#FontSetting-int-int-com.aspose.cells.WorksheetCollection-) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Devuelve la fuente de este objeto. |
| [getLength()](#getLength--) | Obtiene la longitud de los caracteres. |
| [getStartIndex()](#getStartIndex--) | Obtiene el índice de inicio de los caracteres. |
| [getTextOptions()](#getTextOptions--) | Devuelve las opciones de texto. |
| [getType()](#getType--) | Obtiene el tipo de nodo de texto. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Establece el estilo WordArt predefinido. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontSetting(int startIndex, int length, WorksheetCollection sheets) {#FontSetting-int-int-com.aspose.cells.WorksheetCollection-}
```
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int |  |
| length | int |  |
| sheets | [WorksheetCollection](../../com.aspose.cells/worksheetcollection) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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


Devuelve la fuente de este objeto.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Obtiene la longitud de los caracteres.

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Obtiene el índice de inicio de los caracteres.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Devuelve las opciones de texto.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de nodo de texto.

Ver [TextNodeType](../../com.aspose.cells/textnodetype).

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


Establece el estilo WordArt predefinido.

**Remarks**

Solo para el texto de forma/gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). El estilo WordArt predefinido. |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

