---
title: "Range"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das einen Zellbereich innerhalb einer Tabellenkalkulation darstellt."
type: docs
url: /de/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Kapselt das Objekt, das einen Zellbereich innerhalb einer Tabellenkalkulation darstellt.

**Remarks**

Die Range-Klasse bezeichnet einen Bereich einer Excel‑Tabelle. Damit können Sie den Bereich formatieren und dessen Wert festlegen. Und Sie können den Excel‑Bereich auch einfach kopieren.

**Example**

Das folgende Beispiel zeigt, wie man einen Bereich erstellt und den Wert des Excel‑Bereichs festlegt.

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
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Klassenkonstruktor. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Klassenkonstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für einen gesamten Bereich an. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Füllt den Zielbereich automatisch. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Füllt den Zielbereich automatisch. |
| [clear()](#clear--) | Löscht diesen Bereich. |
| [clearComments()](#clearComments--) | Löscht die Kommentare dieses Bereichs. |
| [clearContents()](#clearContents--) | Löscht den Inhalt dieses Bereichs. |
| [clearFormats()](#clearFormats--) | Löscht die Formate dieses Bereichs. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Entfernt nur Hyperlinks. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Kopieren des Bereichs mit Sonderoptionen für Einfügen. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Kopiert Zellen­daten (einschließlich Formeln) aus einem Quellbereich. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Kopiert Stil‑Einstellungen aus einem Quellbereich. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Kopiert den Zellenwert aus einem Quellbereich. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Liest das [Cell](../../com.aspose.cells/cell)-Objekt in diesem Bereich. |
| [getAddress()](#getAddress--) | Liest die Adresse des Bereichs. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Liest das [Cell](../../com.aspose.cells/cell)-Objekt oder null in diesem Bereich. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Liest die Anzahl der Spalten im Bereich. |
| [getColumnWidth()](#getColumnWidth--) | Setzt oder liest die Spaltenbreite dieses Bereichs |
| [getCurrentRegion()](#getCurrentRegion--) | Gibt ein Range‑Objekt zurück, das die aktuelle Region darstellt. |
| [getEntireColumn()](#getEntireColumn--) | Gibt ein Range-Objekt zurück, das die gesamte Spalte (oder Spalten) darstellt, die den angegebenen Bereich enthält. |
| [getEntireRow()](#getEntireRow--) | Gibt ein Range-Objekt zurück, das die gesamte Zeile (oder Zeilen) darstellt, die den angegebenen Bereich enthält. |
| [getFirstColumn()](#getFirstColumn--) | Gibt den Index der ersten Spalte des Bereichs zurück. |
| [getFirstRow()](#getFirstRow--) | Gibt den Index der ersten Zeile des Bereichs zurück. |
| [getHeight()](#getHeight--) | Gibt die Breite eines Bereichs in Punkten zurück. |
| [getHyperlinks()](#getHyperlinks--) | Gibt alle Hyperlinks im Bereich zurück. |
| [getLeft()](#getLeft--) | Gibt den Abstand in Punkten von der linken Kante der Spalte A zur linken Kante des Bereichs zurück. |
| [getName()](#getName--) | Gibt den Namen des Bereichs zurück. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Gibt den [Range](../../com.aspose.cells/range)-Bereich über einen Offset zurück. |
| [getRefersTo()](#getRefersTo--) | Gibt das 'refers to' des Bereichs zurück. |
| [getRowCount()](#getRowCount--) | Gibt die Anzahl der Zeilen im Bereich zurück. |
| [getRowHeight()](#getRowHeight--) | Setzt oder gibt die Höhe der Zeilen in diesem Bereich zurück. |
| [getTop()](#getTop--) | Gibt den Abstand in Punkten von der oberen Kante der Zeile 1 zur oberen Kante des Bereichs zurück. |
| [getValue()](#getValue--) | Gibt den Wert des Bereichs zurück. |
| [getWidth()](#getWidth--) | Gibt die Breite eines Bereichs in Punkten zurück. |
| [getWorksheet()](#getWorksheet--) | Gibt das [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)Objekt zurück, das diesen Bereich enthält. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Gibt ein [Range](../../com.aspose.cells/range)-Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt. |
| [isBlank()](#isBlank--) | Gibt an, ob der Bereich Werte enthält. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Gibt an, ob der Bereich sich überschneidet. |
| [iterator()](#iterator--) | Gibt den Enumerator für Zellen in diesem Range zurück. |
| [merge()](#merge--) | Kombiniert einen Zellbereich zu einer einzelnen Zelle. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Verschiebt den aktuellen Bereich zum Zielbereich. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Setzt einen Wert in den Bereich; falls nötig wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Setzt oder liest die Spaltenbreite dieses Bereichs |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Setzt innere Rahmen des Bereichs. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen des Bereichs. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Setzt den Umrissrahmen um einen Zellbereich. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Setzt den Umrissrahmen um einen Zellbereich. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Legt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe fest. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Legt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe fest. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Legt Umrandungsrahmen um einen Zellbereich fest. |
| [setRowHeight(double value)](#setRowHeight-double-) | Setzt oder gibt die Höhe der Zeilen in diesem Bereich zurück. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Legt den Stil des Bereichs fest. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Wendet den Zellenstil an. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Legt den Wert des Bereichs fest. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Konvertiert den Bereich in HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Konvertiert den Bereich in ein Bild. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Konvertiert den Bereich in einen JSON-Wert. |
| [toString()](#toString--) | Gibt einen String zurück, der das aktuelle Range-Objekt darstellt. |
| [transpose()](#transpose--) | Transponiert (dreht) Daten von Zeilen zu Spalten oder umgekehrt. |
| [unMerge()](#unMerge--) | Löst zusammengeführte Zellen dieses Bereichs. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Gibt die Vereinigung zweier Bereiche zurück. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Gibt das Ergebnis der Vereinigung zweier Bereiche zurück. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Gibt das Ergebnis der Vereinigung zweier Bereiche zurück. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Klassenkonstruktor.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Klassenkonstruktor.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | int | Erste Spalte dieses Bereichs (nullbasiert) |
| rowNumber | int | Anzahl der Zeilen (einsbasiert) |
| columnNumber | int | Anzahl der Spalten (beginnend bei 1) |
| cells | [Cells](../../com.aspose.cells/cells) | Das Range-Objekt gehört zu diesem Cells-Objekt |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Adresse | java.lang.String | Adresse des Hyperlinks. |
| textToDisplay | java.lang.String | Der Text, der für den angegebenen Hyperlink angezeigt wird. |
| screenTip | java.lang.String | Der ScreenTip-Text für den angegebenen Hyperlink. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Wendet Formate für einen gesamten Bereich an.

**Remarks**

Jede Zelle in diesem Bereich enthält ein [Style](../../com.aspose.cells/style)-Objekt. Daher ist diese Methode speicherintensiv. Bitte verwenden Sie sie vorsichtig.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Füllt den Zielbereich automatisch.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | der Zielbereich. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Füllt den Zielbereich automatisch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | Der Zielbereich. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). Der Autoausfülltyp. |

### clear() {#clear--}
```
public void clear()
```


Löscht diesen Bereich.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Löscht die Kommentare dieses Bereichs.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Löscht den Inhalt dieses Bereichs.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Löscht die Formate dieses Bereichs.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Entfernt nur Hyperlinks.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| clearFormat | boolean | Gibt an, ob das Format von Hyperlinks gelöscht werden soll. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Quell-[Range](../../com.aspose.cells/range)-Objekt. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Kopieren des Bereichs mit Sonderoptionen für Einfügen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der Quellbereich. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Die Optionen für Einfügen Spezial. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Kopiert Zellen­daten (einschließlich Formeln) aus einem Quellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Quell-[Range](../../com.aspose.cells/range)-Objekt. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Kopiert Stil‑Einstellungen aus einem Quellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Quell-[Range](../../com.aspose.cells/range)-Objekt. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Kopiert den Zellenwert aus einem Quellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Quell-[Range](../../com.aspose.cells/range)-Objekt. |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Liest das [Cell](../../com.aspose.cells/cell)-Objekt in diesem Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Zeilenversatz in diesem Bereich, nullbasiert. |
| columnOffset | int | Spaltenversatz in diesem Bereich, nullbasiert. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Liest die Adresse des Bereichs.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Liest das [Cell](../../com.aspose.cells/cell)-Objekt oder null in diesem Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Zeilenversatz in diesem Bereich, nullbasiert. |
| columnOffset | int | Spaltenversatz in diesem Bereich, nullbasiert. |

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


Liest die Anzahl der Spalten im Bereich.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Setzt oder liest die Spaltenbreite dieses Bereichs

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt. Die aktuelle Region ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt wird.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Gibt ein Range-Objekt zurück, das die gesamte Spalte (oder Spalten) darstellt, die den angegebenen Bereich enthält.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Gibt ein Range-Objekt zurück, das die gesamte Zeile (oder Zeilen) darstellt, die den angegebenen Bereich enthält.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Gibt den Index der ersten Spalte des Bereichs zurück.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Gibt den Index der ersten Zeile des Bereichs zurück.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Gibt die Breite eines Bereichs in Punkten zurück.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Gibt alle Hyperlinks im Bereich zurück.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


Gibt den Abstand in Punkten von der linken Kante der Spalte A zur linken Kante des Bereichs zurück.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen des Bereichs zurück.

**Remarks**

Benannte Bereiche werden unterstützt. Zum Beispiel,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Gibt den [Range](../../com.aspose.cells/range)-Bereich über einen Offset zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | int | Zeilenversatz in diesem Bereich, nullbasiert. |
| columnOffset | int | Spaltenversatz in diesem Bereich, nullbasiert. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Gibt das 'refers to' des Bereichs zurück.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Gibt die Anzahl der Zeilen im Bereich zurück.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Setzt oder gibt die Höhe der Zeilen in diesem Bereich zurück.

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


Gibt den Abstand in Punkten von der oberen Kante der Zeile 1 zur oberen Kante des Bereichs zurück.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Gibt den Wert des Bereichs zurück.

**Remarks**

Wenn der Bereich mehrere Zellen enthält, sollte das zurückgegebene/angewendete Objekt Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Gibt die Breite eines Bereichs in Punkten zurück.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Gibt das [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--)Objekt zurück, das diesen Bereich enthält.

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


Gibt ein [Range](../../com.aspose.cells/range)-Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt.

**Remarks**

Wenn die beiden Bereiche nicht überlappen, wird null zurückgegeben.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der sich überschneidende Bereich. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Gibt an, ob der Bereich Werte enthält.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Gibt an, ob der Bereich sich überschneidet.

**Remarks**

Wenn die beiden Bereiche nicht im selben Arbeitsblatt liegen, wird false zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der Bereich. |

**Returns:**
boolean - Ob der Bereich sich überschneidet.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt den Enumerator für Zellen in diesem Range zurück.

**Remarks**

Beim Durchlaufen von Elementen mit dem zurückgegebenen Enumerator sollte die Zellen‑Sammlung nicht verändert werden (z. B. Operationen, die dazu führen, dass neue Cell/Row erzeugt oder vorhandene Cell/Row gelöscht werden). Andernfalls kann der Enumerator möglicherweise nicht alle Zellen korrekt durchlaufen (einige Elemente können mehrfach durchlaufen oder übersprungen werden).

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
java.util.Iterator - Der Zellen‑Enumerator
### merge() {#merge--}
```
public void merge()
```


Kombiniert einen Zellbereich zu einer einzelnen Zelle.

**Remarks**

Referenzieren Sie die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Verschiebt den aktuellen Bereich zum Zielbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destRow | int | Die Startzeile des Zielbereichs. |
| destColumn | int | Die Startspalte des Zielbereichs. |

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


Setzt einen Wert in den Bereich; falls nötig wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |
| isConverted | boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |
| setStyle | boolean | True: das Zahlenformat auf den Zellenstil setzen, wenn in einen anderen Datentyp konvertiert wird |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Setzt oder liest die Spaltenbreite dieses Bereichs

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Setzt innere Rahmen des Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Im Border-Typ kann nur [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) und [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL) verwendet werden. |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Der Rahmenstil. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Die Farbe des Rahmens. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Setzt den Namen des Bereichs.

**Remarks**

Benannte Bereiche werden unterstützt. Zum Beispiel,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Setzt den Umrissrahmen um einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Randkante. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstil. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Randfarbe. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Setzt den Umrissrahmen um einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Randkante. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstil. |
| borderColor | [Color](../../com.aspose.cells/color) | Randfarbe. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Legt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstil. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Randfarbe. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Legt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstil. |
| borderColor | [Color](../../com.aspose.cells/color) | Randfarbe. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Legt Umrandungsrahmen um einen Zellbereich fest.

**Remarks**

Sowohl die Länge von borderStyles als auch von borderStyles muss 4 betragen. Die Reihenfolge von borderStyles und borderStyles muss oben, unten, links, rechts sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstile. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Randfarben. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Setzt oder gibt die Höhe der Zeilen in diesem Bereich zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Legt den Stil des Bereichs fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Style-Objekt. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Wendet den Zellenstil an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Der Zellenstil. |
| explicitFlag | boolean | True, überschreibt nur Formatierungen, die explizit festgelegt wurden. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Legt den Wert des Bereichs fest.

**Remarks**

Wenn der Bereich mehrere Zellen enthält, sollte das zurückgegebene/angewendete Objekt Object[][].

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Konvertiert den Bereich in HTML.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Optionen zum Konvertieren des Bereichs in HTML. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Konvertiert den Bereich in ein Bild.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Die Optionen zum Konvertieren dieses Bereichs in ein Bild |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Konvertiert den Bereich in einen JSON-Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Die Optionen zum Konvertieren |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Gibt einen String zurück, der das aktuelle Range-Objekt darstellt.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Transponiert (dreht) Daten von Zeilen zu Spalten oder umgekehrt.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Löst zusammengeführte Zellen dieses Bereichs.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


Gibt die Vereinigung zweier Bereiche zurück.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Range.UnionRanges(). Diese Methode wird 12 Monate nach November 2023 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der Bereich |

**Returns:**
java.util.ArrayList - Die Vereinigung zweier Bereiche.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


Gibt das Ergebnis der Vereinigung zweier Bereiche zurück.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Range.UnionRanges(). Diese Methode wird 12 Monate nach Mai 2024 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der Bereich |

**Returns:**
com.aspose.cells.Range[] - Die Vereinigung zweier Bereiche.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


Gibt das Ergebnis der Vereinigung zweier Bereiche zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Der Bereich |

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

