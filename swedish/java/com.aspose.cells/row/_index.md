---
title: "Rad"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en enda rad i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Representerar en enda rad i ett kalkylblad.

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
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för en hel rad. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Kopiera inställningar för raden, såsom stil, höjd, synlighet, ...etc. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Kontrollerar om detta objekt refererar till samma rad som ett annat radobjekt. |
| [equals(Object obj)](#equals-java.lang.Object-) | Kontrollerar om detta objekt refererar till samma rad som ett annat. |
| [get(int column)](#get-int-) | Hämtar cellen. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Hämta cellen med ett specifikt index i cellsamlingen för denna rad. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Hämtar cellen eller null på det specifika indexet. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Hämtar det första cellobjektet i raden. |
| [getFirstDataCell()](#getFirstDataCell--) | Hämtar den första icke-tomma cellen i raden. |
| [getGroupLevel()](#getGroupLevel--) | Hämtar gruppnivån för raden. |
| [getHeight()](#getHeight--) | Hämtar radens höjd i enheten Points. |
| [getIndex()](#getIndex--) | Hämtar indexet för denna rad. |
| [getLastCell()](#getLastCell--) | Hämtar det sista cellobjektet i raden. |
| [getLastDataCell()](#getLastDataCell--) | Hämtar den sista icke-tomma cellen i raden. |
| [getStyle()](#getStyle--) | Hämtar stil för den här raden. |
| [hasCustomStyle()](#hasCustomStyle--) | Anger om den här raden har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från arbetsboken). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Anger om raden innehåller någon data |
| [isCollapsed()](#isCollapsed--) | om raden är hopfälld |
| [isHeightMatched()](#isHeightMatched--) | Anger om radhöjden matchar den aktuella standardteckensnittinställningen i arbetsboken. |
| [isHidden()](#isHidden--) | Anger om raden är dold. |
| [iterator()](#iterator--) | Hämtar cellernas enumerator |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Hämtar en enumerator som itererar celler genom den här raden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | om raden är hopfälld |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Hämtar gruppnivån för raden. |
| [setHeight(double value)](#setHeight-double-) | Ställer in radhöjden i enheten punkter. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Anger om radhöjden matchar den aktuella standardteckensnittinställningen i arbetsboken. |
| [setHidden(boolean value)](#setHidden-boolean-) | Anger om raden är dold. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Ställer in stil för den här raden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tillämpar format för en hel rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Kopiera inställningar för raden, såsom stil, höjd, synlighet, ...etc.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | källraden vars inställningar kommer att kopieras till denna |
| checkStyle | boolean | om stil ska kontrolleras och samlas in. Gäller endast och behövs när två radobjekt tillhör olika arbetsböcker och stilarna i de två arbetsböckerna är olika. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Kontrollerar om detta objekt refererar till samma rad som ett annat radobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | ett annat radobjekt |

**Returns:**
boolesk - true om två radobjekt refererar till samma rad.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Kontrollerar om detta objekt refererar till samma rad som ett annat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | ett annat objekt |

**Returns:**
boolesk - true om två objekt refererar till samma rad.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Hämtar cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Hämta cellen med ett specifikt index i cellsamlingen för denna rad.

**Remarks**

För att gå igenom alla celler i sekvens utan ändring, ger användning av [iterator()](../../com.aspose.cells/row\#iterator--) bättre prestanda än att använda den här metoden för att hämta cellen en i taget.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet (positionen) för cellen i cellsamlingen för den här raden. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Hämtar cellen eller null på det specifika indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Hämtar det första cellobjektet i raden.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Hämtar den första icke-tomma cellen i raden.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Hämtar gruppnivån för raden.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Hämtar radens höjd i enheten Points.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar indexet för denna rad.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Hämtar det sista cellobjektet i raden.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Hämtar den sista icke-tomma cellen i raden.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hämtar stil för den här raden.

**Remarks**

Att ändra det returnerade stilobjektet direkt har ingen effekt för den här raden eller några celler i den här raden. Du måste anropa [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) eller [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) metoden för att tillämpa ändringen på den här raden.

Radsstil är den stil som kommer att ärvas av celler i den här raden (de celler som inte har anpassade stilinställningar, såsom befintliga celler som inte har fått stil uttryckligen, eller de som inte har instansierats)

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Anger om den här raden har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från arbetsboken).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Anger om raden innehåller någon data

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


om raden är hopfälld

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Anger om radhöjden matchar den aktuella standardteckensnittinställningen i arbetsboken. True för denna egenskap betyder också att radhöjden är "automatisk" utan att ett anpassat höjdvärde har satts av användaren.

**Remarks**

När den här egenskapen är sann, om innehållet i den här raden ändras, måste radens höjd vanligtvis omberäknas (t.ex. med [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) för att få samma resultat som visas i MS Excel när du öppnar arbetsboken i den.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Anger om raden är dold.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar cellernas enumerator

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Cellräknaren som kommer att gå igenom alla befintliga celler i den här raden.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Hämtar en enumerator som itererar celler genom den här raden.

**Remarks**

Om raden kommer att modifieras (genom operationer som kan orsaka att en ny Cell skapas eller en befintlig Cell tas bort) under genomgången med räknaren, bör en synkroniserad räknare användas i stället för en normal räknare så att genomgången kan fortsätta från positionen precis efter den som har traverserats av den senaste MoveNext(). Dock, förutom fördelen att inget element hoppar över eller traverseras flera gånger, är nackdelen med den synkroniserade räknaren att prestandan blir något försämrad jämfört med en normal räknare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omvänd | boolean | om celler ska räknas i omvänd ordning |
| synk | boolean | om den returnerade räknaren ska kontrollera ändringar av celler i den här raden och hålla sig synkroniserad med den. |

**Returns:**
java.util.Iterator - Cellräknaren som kommer att gå igenom alla befintliga celler i den här raden.
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


om raden är hopfälld

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Hämtar gruppnivån för raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Ställer in radhöjden i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Anger om radhöjden matchar den aktuella standardteckensnittinställningen i arbetsboken. True för denna egenskap betyder också att radhöjden är "automatisk" utan att ett anpassat höjdvärde har satts av användaren.

**Remarks**

När den här egenskapen är sann, om innehållet i den här raden ändras, måste radens höjd vanligtvis omberäknas (t.ex. med [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) för att få samma resultat som visas i MS Excel när du öppnar arbetsboken i den.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Anger om raden är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Ställer in stil för den här raden.

**Remarks**

Denna metod sätter bara den angivna stilen som standardstil för den här raden, utan att ändra stilinställningarna för befintliga celler i raden. För att samtidigt uppdatera stilinställningarna för befintliga celler till den specificerade stilen, använd [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | stilen som ska användas som standardstil för celler i den här raden. |

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

