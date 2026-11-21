---
title: "Range"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar ett cellområde i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Inkapslar objektet som representerar ett cellområde i ett kalkylblad.

**Remarks**

Klassen Range betecknar ett område i ett Excel‑kalkylblad. Med detta kan du formatera och ange värdet för området. Och du kan också enkelt kopiera ett Excel‑område också.

**Example**

Följande exempel visar hur man skapar ett område och anger värdet för Excel‑området.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Klasskonstruktor. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Klasskonstruktor. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Lägger till en hyperlänk i en angiven cell eller ett cellområde. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för ett helt område. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Fyll automatiskt målområdet. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Fyll automatiskt målområdet. |
| [clear()](#clear--) | Rensar detta område. |
| [clearComments()](#clearComments--) | Rensar kommentarerna i detta område. |
| [clearContents()](#clearContents--) | Rensar innehållet i detta område. |
| [clearFormats()](#clearFormats--) | Rensar formaten i detta område. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Tar bara bort hyperlänkar. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Kopierar data (inklusive formler), formatering, ritobjekt etc. från ett källområde. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Kopierar området med specialklistra‑alternativ. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Kopierar celldata (inklusive formler) från ett källområde. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Kopierar stilinställningar från ett källområde. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Kopierar cellvärde från ett källområde. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Hämtar [Cell](../../com.aspose.cells/cell)-objekt i detta område. |
| [getAddress()](#getAddress--) | Hämtar adressen för området. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Hämtar [Cell](../../com.aspose.cells/cell)-objekt eller null i detta område. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Hämtar antalet kolumner i området. |
| [getColumnWidth()](#getColumnWidth--) | Ställer in eller hämtar kolumnbredden för detta område |
| [getCurrentRegion()](#getCurrentRegion--) | Returnerar ett Range‑objekt som representerar den aktuella regionen. |
| [getEntireColumn()](#getEntireColumn--) | Hämtar ett Range‑objekt som representerar hela kolumnen (eller kolumnerna) som innehåller det angivna området. |
| [getEntireRow()](#getEntireRow--) | Hämtar ett Range‑objekt som representerar hela raden (eller raderna) som innehåller det angivna området. |
| [getFirstColumn()](#getFirstColumn--) | Hämtar indexet för den första kolumnen i området. |
| [getFirstRow()](#getFirstRow--) | Hämtar indexet för den första raden i området. |
| [getHeight()](#getHeight--) | Hämtar bredden på ett område i punkter. |
| [getHyperlinks()](#getHyperlinks--) | Hämtar alla hyperlänkar i området. |
| [getLeft()](#getLeft--) | Hämtar avståndet, i punkter, från vänsterkanten av kolumn A till vänsterkanten av området. |
| [getName()](#getName--) | Hämtar namnet på området. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Hämtar [Range](../../com.aspose.cells/range) område med förskjutning. |
| [getRefersTo()](#getRefersTo--) | Hämtar vad området refererar till. |
| [getRowCount()](#getRowCount--) | Hämtar antalet rader i området. |
| [getRowHeight()](#getRowHeight--) | Ställer in eller hämtar höjden på rader i detta område |
| [getTop()](#getTop--) | Hämtar avståndet, i punkter, från överkanten av rad 1 till överkanten av området. |
| [getValue()](#getValue--) | Hämtar värdet på området. |
| [getWidth()](#getWidth--) | Hämtar bredden på ett område i punkter. |
| [getWorksheet()](#getWorksheet--) | Hämtar [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)objektet som innehåller detta område. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Returnerar ett [Range](../../com.aspose.cells/range) objekt som representerar den rektangulära skärningen av två områden. |
| [isBlank()](#isBlank--) | Indikerar om området innehåller värden. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Indikerar om området intersectar. |
| [iterator()](#iterator--) | Hämtar enumeratorn för celler i detta område. |
| [merge()](#merge--) | Kombinerar ett område av celler till en enda cell. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Flytta det aktuella området till destinationsområdet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Sätter ett värde i området, om lämpligt kommer värdet att konverteras till en annan datatyp och cellens talformat återställas. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Ställer in eller hämtar kolumnbredden för detta område |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Ställ in de inre kantlinjerna för området. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på området. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Ställer in konturkant runt ett område av celler. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Ställer in konturkant runt ett område av celler. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Ställer in konturkantlinjer runt ett område av celler med samma kantstil och färg. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Ställer in konturkantlinjer runt ett område av celler med samma kantstil och färg. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Ställer in konturkantlinjer runt ett område av celler. |
| [setRowHeight(double value)](#setRowHeight-double-) | Ställer in eller hämtar höjden på rader i detta område |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Ställer in stilen för området. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Applicera cellstilen. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ställer in värdet för området. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Konvertera området till HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Konverterar området till en bild. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Konvertera området till JSON‑värde. |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella Range-objektet. |
| [transpose()](#transpose--) | Transponera (rotera) data från rader till kolumner eller vice versa. |
| [unMerge()](#unMerge--) | Ta bort sammanslagning av sammanslagna celler i detta område. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Returnerar unionen av två områden. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Returnerar unionsresultatet av två områden. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Returnerar unionsresultatet av två områden. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Klasskonstruktor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Intervallet. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Klasskonstruktor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta område (nollbaserat) |
| rowNumber | int | Antal rader (enbaserat) |
| columnNumber | int | Antal kolumner (enbaserat) |
| cells | [Cells](../../com.aspose.cells/cells) | Range‑objektet tillhör detta Cells‑objekt |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Lägger till en hyperlänk i en angiven cell eller ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | java.lang.String | Adress för hyperlänken. |
| textToDisplay | java.lang.String | Texten som ska visas för den angivna hyperlänken. |
| screenTip | java.lang.String | ScreenTip-texten för den angivna hyperlänken. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tillämpar format för ett helt område.

**Remarks**

Varje cell i detta område kommer att innehålla ett [Style](../../com.aspose.cells/style)-objekt. Så detta är en minneskrävande metod. Använd den med försiktighet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Fyll automatiskt målområdet.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | det målområdet. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Fyll automatiskt målområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | Det målområdet. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). Den automatiska fyllningstypen. |

### clear() {#clear--}
```
public void clear()
```


Rensar detta område.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Rensar kommentarerna i detta område.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Rensar innehållet i detta område.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Rensar formaten i detta område.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Tar bara bort hyperlänkar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| clearFormat | boolean | Indikerar om formatet för hyperlänkar ska rensas. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Kopierar data (inklusive formler), formatering, ritobjekt etc. från ett källområde.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Källa [Range](../../com.aspose.cells/range)-objekt. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Kopierar området med specialklistra‑alternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Källintervallet. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Klistra in specialalternativ. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Kopierar celldata (inklusive formler) från ett källområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Källa [Range](../../com.aspose.cells/range)-objekt. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Kopierar stilinställningar från ett källområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Källa [Range](../../com.aspose.cells/range)-objekt. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Kopierar cellvärde från ett källområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Källa [Range](../../com.aspose.cells/range)-objekt. |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Hämtar [Cell](../../com.aspose.cells/cell)-objekt i detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radförskjutning i detta område, nollbaserat. |
| columnOffset | int | Kolumnförskjutning i detta område, nollbaserat. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Hämtar adressen för området.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Hämtar [Cell](../../com.aspose.cells/cell)-objekt eller null i detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radförskjutning i detta område, nollbaserat. |
| columnOffset | int | Kolumnförskjutning i detta område, nollbaserat. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Hämtar antalet kolumner i området.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Ställer in eller hämtar kolumnbredden för detta område

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Returnerar ett Range‑objekt som representerar den aktuella regionen. Den aktuella regionen är ett område som begränsas av någon kombination av tomma rader och tomma kolumner.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Hämtar ett Range‑objekt som representerar hela kolumnen (eller kolumnerna) som innehåller det angivna området.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Hämtar ett Range‑objekt som representerar hela raden (eller raderna) som innehåller det angivna området.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Hämtar indexet för den första kolumnen i området.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Hämtar indexet för den första raden i området.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Hämtar bredden på ett område i punkter.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Hämtar alla hyperlänkar i området.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


Hämtar avståndet, i punkter, från vänsterkanten av kolumn A till vänsterkanten av området.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på området.

**Remarks**

Namngivet område stöds. Till exempel,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Hämtar [Range](../../com.aspose.cells/range) område med förskjutning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radförskjutning i detta område, nollbaserat. |
| columnOffset | int | Kolumnförskjutning i detta område, nollbaserat. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Hämtar vad området refererar till.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Hämtar antalet rader i området.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Ställer in eller hämtar höjden på rader i detta område

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


Hämtar avståndet, i punkter, från överkanten av rad 1 till överkanten av området.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdet på området.

**Remarks**

Om området innehåller flera celler, bör det returnerade/tillämpade objektet vara Object[][]

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Hämtar bredden på ett område i punkter.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hämtar [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)objektet som innehåller detta område.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


Returnerar ett [Range](../../com.aspose.cells/range) objekt som representerar den rektangulära skärningen av två områden.

**Remarks**

Om de två områdena inte skär varandra, returneras null.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Det skärande området. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indikerar om området innehåller värden.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Indikerar om området intersectar.

**Remarks**

Om de två områdena inte är i samma kalkylblad, returneras false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Intervallet. |

**Returns:**
boolean - Om området skär varandra.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar enumeratorn för celler i detta område.

**Remarks**

När element traverseras med den returnerade Enumerator bör cellsamlingen inte modifieras (såsom operationer som skapar nya Cell/Row eller tar bort befintliga Cell/Row). Annars kan enumeratorn misslyckas med att traversera alla celler korrekt (vissa element kan traverseras flera gånger eller hoppas över).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Cellernas enumerator
### merge() {#merge--}
```
public void merge()
```


Kombinerar ett område av celler till en enda cell.

**Remarks**

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i intervallet.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Flytta det aktuella området till destinationsområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destRow | int | Startraden för målområdet. |
| destColumn | int | Startkolumnen för målområdet. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Sätter ett värde i området, om lämpligt kommer värdet att konverteras till en annan datatyp och cellens talformat återställas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |
| isConverted | boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | boolean | True: sätt talformatet till cellens stil när du konverterar till annan datatyp |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Ställer in eller hämtar kolumnbredden för detta område

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Ställ in de inre kantlinjerna för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Inom border-typen kan endast vara [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) och [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL). |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilen. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Färgen på kanten. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på området.

**Remarks**

Namngivet område stöds. Till exempel,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Ställer in konturkant runt ett område av celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Borderkant. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilen. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Borderfärg. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Ställer in konturkant runt ett område av celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Borderkant. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilen. |
| borderColor | [Color](../../com.aspose.cells/color) | Borderfärg. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Ställer in konturkantlinjer runt ett område av celler med samma kantstil och färg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilen. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Borderfärg. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Ställer in konturkantlinjer runt ett område av celler med samma kantstil och färg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilen. |
| borderColor | [Color](../../com.aspose.cells/color) | Borderfärg. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Ställer in konturkantlinjer runt ett område av celler.

**Remarks**

Både längden på borderStyles och borderStyles måste vara 4. Ordningen på borderStyles och borderStyles måste vara top,bottom,left,right

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilar. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Borderfärger. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Ställer in eller hämtar höjden på rader i detta område

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Ställer in stilen för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style-objektet. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Applicera cellstilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Cellstilen. |
| explicitFlag | boolean | Sant, endast skriva över formatering som är explicit angiven. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Ställer in värdet för området.

**Remarks**

Om området innehåller flera celler, bör det returnerade/tillämpade objektet vara Object[][]

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Konvertera området till HTML.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Alternativ för att konvertera område till html. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Konverterar området till en bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Alternativen för att konvertera detta område till bild |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Konvertera området till JSON‑värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Alternativen för konvertering |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella Range-objektet.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Transponera (rotera) data från rader till kolumner eller vice versa.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Ta bort sammanslagning av sammanslagna celler i detta område.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


Returnerar unionen av två områden.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Range.UnionRanges()-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Området |

**Returns:**
java.util.ArrayList - Unionen av två områden.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


Returnerar unionsresultatet av två områden.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Range.UnionRanges()-metoden. Denna metod kommer att tas bort 12 månader senare från och med maj 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Området |

**Returns:**
com.aspose.cells.Range[] - Unionen av två områden.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


Returnerar unionsresultatet av två områden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Området |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
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

