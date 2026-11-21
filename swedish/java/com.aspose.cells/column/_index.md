---
title: "Kolumn"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en enskild kolumn i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Representerar en enskild kolumn i ett kalkylblad.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för en hel kolumn. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Hämtar gruppnivån för kolumnen. |
| [getIndex()](#getIndex--) | Hämtar indexet för denna kolumn. |
| [getStyle()](#getStyle--) | Hämtar stilen för denna kolumn. |
| [getWidth()](#getWidth--) | Hämtar kolumnbredden i tecken. |
| [hasCustomStyle()](#hasCustomStyle--) | Indikerar om denna kolumn har anpassade stilinställningar(annorlunda än standardinställningen som ärvs från arbetsboken). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | om kolumnen är kollapsad |
| [isHidden()](#isHidden--) | Indikerar om kolumnen är dold. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | om kolumnen är kollapsad |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Hämtar gruppnivån för kolumnen. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indikerar om kolumnen är dold. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Ställer in stilen för denna kolumn. |
| [setWidth(double value)](#setWidth-double-) | Ställer in kolumnbredden i tecken. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tillämpar format för en hel kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Hämtar gruppnivån för kolumnen.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar indexet för denna kolumn.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hämtar stilen för denna kolumn.

**Remarks**

Att modifiera det returnerade stilobjektet direkt har ingen effekt för denna kolumn eller några celler i denna kolumn. Du måste anropa [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) eller [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) metoden för att tillämpa ändringen på denna kolumn.

Kolumnens stil är den stil som kommer att ärvas av celler i denna kolumn(de celler som inte har anpassade stilinställningar, såsom befintliga celler som inte har fått stil explicit, eller de som ännu inte har instansierats).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Hämtar kolumnbredden i tecken.

**Remarks**

För kalkylblad mäts kolumnbredden som antalet tecken av den maximala siffrabredden för siffrorna 0~9 när de renderas i det normala stilens teckensnitt.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indikerar om denna kolumn har anpassade stilinställningar(annorlunda än standardinställningen som ärvs från arbetsboken).

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


om kolumnen är kollapsad

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indikerar om kolumnen är dold.

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


om kolumnen är kollapsad

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Hämtar gruppnivån för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indikerar om kolumnen är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Ställer in stilen för denna kolumn.

**Remarks**

Denna metod ställer endast in den angivna stilen som standardstil för denna kolumn, utan att ändra stilinställningarna för befintliga celler i kolumnen. För att uppdatera stilinställningarna för befintliga celler till den angivna stilen samtidigt, vänligen använd [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | stilen som ska användas som standardstil för celler i denna kolumn. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Ställer in kolumnbredden i tecken.

**Remarks**

För kalkylblad mäts kolumnbredden som antalet tecken av den maximala siffrabredden för siffrorna 0~9 när de renderas i det normala stilens teckensnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

