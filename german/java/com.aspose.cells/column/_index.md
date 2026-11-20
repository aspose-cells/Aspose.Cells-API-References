---
title: "Spalte"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine einzelne Spalte in einem Arbeitsblatt dar."
type: docs
url: /de/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Stellt eine einzelne Spalte in einem Arbeitsblatt dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für eine gesamte Spalte an. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Ermittelt die Gruppenebene der Spalte. |
| [getIndex()](#getIndex--) | Ermittelt den Index dieser Spalte. |
| [getStyle()](#getStyle--) | Ermittelt den Stil dieser Spalte. |
| [getWidth()](#getWidth--) | Ermittelt die Spaltenbreite in Zeichen. |
| [hasCustomStyle()](#hasCustomStyle--) | Gibt an, ob diese Spalte benutzerdefinierte Stileinstellungen hat (anders als die standardmäßige, die von der Arbeitsmappe geerbt wird). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | ob die Spalte zusammengeklappt ist |
| [isHidden()](#isHidden--) | Gibt an, ob die Spalte ausgeblendet ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | ob die Spalte zusammengeklappt ist |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Ermittelt die Gruppenebene der Spalte. |
| [setHidden(boolean value)](#setHidden-boolean-) | Gibt an, ob die Spalte ausgeblendet ist. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Legt den Stil dieser Spalte fest. |
| [setWidth(double value)](#setWidth-double-) | Legt die Spaltenbreite in Zeichen fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Wendet Formate für eine gesamte Spalte an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Ermittelt die Gruppenebene der Spalte.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ermittelt den Index dieser Spalte.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ermittelt den Stil dieser Spalte.

**Remarks**

Das direkte Ändern des zurückgegebenen Stilobjekts hat keine Wirkung für diese Spalte oder deren Zellen. Sie müssen die Methode [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) oder [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) aufrufen, um die Änderung auf diese Spalte anzuwenden.

Der Stil der Spalte ist der Stil, der von den Zellen in dieser Spalte übernommen wird (jene Zellen, die keine benutzerdefinierten Stileinstellungen haben, wie vorhandene Zellen, denen kein Stil explizit zugewiesen wurde, oder solche, die noch nicht instanziiert wurden).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Ermittelt die Spaltenbreite in Zeichen.

**Remarks**

Für Tabellenkalkulationen wird die Spaltenbreite als die Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des normalen Stils dargestellt werden.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Gibt an, ob diese Spalte benutzerdefinierte Stileinstellungen hat (anders als die standardmäßige, die von der Arbeitsmappe geerbt wird).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


ob die Spalte zusammengeklappt ist

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Gibt an, ob die Spalte ausgeblendet ist.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


ob die Spalte zusammengeklappt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Ermittelt die Gruppenebene der Spalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Gibt an, ob die Spalte ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Legt den Stil dieser Spalte fest.

**Remarks**

Diese Methode legt den angegebenen Stil nur als Standardstil für diese Spalte fest, ohne die Stileinstellungen der vorhandenen Zellen in dieser Spalte zu ändern. Um die Stileinstellungen der vorhandenen Zellen gleichzeitig auf den angegebenen Stil zu aktualisieren, verwenden Sie bitte [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Der Stil, der als Standardstil für die Zellen in dieser Spalte verwendet wird. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Legt die Spaltenbreite in Zeichen fest.

**Remarks**

Für Tabellenkalkulationen wird die Spaltenbreite als die Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des normalen Stils dargestellt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

