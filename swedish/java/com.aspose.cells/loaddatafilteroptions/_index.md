---
title: "LoadDataFilterOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att filtrera data när arbetsboken laddas från en mall."
type: docs
url: /sv/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Representerar alternativen för att filtrera data när arbetsboken laddas från en mall.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ALL](#ALL) | Läs in alla |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Läs in inställningar för arbetsbok |
| [CELL_BLANK](#CELL-BLANK) | Läs in celler vars värde är tomt |
| [CELL_BOOL](#CELL-BOOL) | Läs in celler vars värde är boolesk |
| [CELL_DATA](#CELL-DATA) | Läs in celldata inklusive värden, formler och formatering |
| [CELL_ERROR](#CELL-ERROR) | Läs in celler vars värde är fel |
| [CELL_NUMERIC](#CELL-NUMERIC) | Läs in celler vars värde är numeriskt (inklusive datum/tid) |
| [CELL_STRING](#CELL-STRING) | Läs in celler vars värde är en sträng |
| [CELL_VALUE](#CELL-VALUE) | Läs in endast cellvärden (alla värdetyper) |
| [CHART](#CHART) | Läs in diagram |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Läs in villkorlig formatering |
| [DATA_VALIDATION](#DATA-VALIDATION) | Läs in datavalideringar |
| [DEFINED_NAMES](#DEFINED-NAMES) | Läs in definierade namnobjekt |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Läs in dokumentegenskaper |
| [DRAWING](#DRAWING) | Ritobjekt (inklusive Diagram, Bild, OleObject och alla andra ritobjekt) |
| [FORMULA](#FORMULA) | Läs in cellformler. |
| [HYPERLINKS](#HYPERLINKS) | Läs in hyperlänkar |
| [MERGED_AREA](#MERGED-AREA) | Läs in sammanslagna celler |
| [NONE](#NONE) | Läs in inget för bladdata |
| [OLE_OBJECT](#OLE-OBJECT) | Läs in OleObjects |
| [PICTURE](#PICTURE) | Läs in bilder |
| [PIVOT_TABLE](#PIVOT-TABLE) | Läs in pivottabeller |
| [REVISION](#REVISION) | Läs in revisionsloggar |
| [SETTINGS](#SETTINGS) | Läs in inställningar för arbetsbok och arbetsblad |
| [SHAPE](#SHAPE) | Läs in former |
| [SHEET_DATA](#SHEET-DATA) | Läs in all data för arbetsblad, såsom celldata, inställningar, objekt, ...etc. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Läs in inställningar för arbetsblad |
| [STRUCTURE](#STRUCTURE) | Läs in strukturen för arbetsboken |
| [STYLE](#STYLE) | Läs in stilar för cellformatering |
| [TABLE](#TABLE) | Läs in tabeller |
| [VBA](#VBA) | Läs in VBA-projekt |
| [XML_MAP](#XML-MAP) | Läs in XmlMap |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Läs in alla

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Läs in inställningar för arbetsbok

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Läs in celler vars värde är tomt

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Läs in celler vars värde är boolesk

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Läs in celldata inklusive värden, formler och formatering

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Läs in celler vars värde är fel

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Läs in celler vars värde är numeriskt (inklusive datum/tid)

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Läs in celler vars värde är en sträng

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Läs in endast cellvärden (alla värdetyper)

### CHART {#CHART}
```
public static final int CHART
```


Läs in diagram

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Läs in villkorlig formatering

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Läs in datavalideringar

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Läs in definierade namnobjekt

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Läs in dokumentegenskaper

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Ritobjekt (inklusive Diagram, Bild, OleObject och alla andra ritobjekt)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Läs in cellformler.

**Remarks**

Generellt måste definierade namnobjekt (DefinedNames) också läsas in när formler läses in eftersom de kan refereras av formler. Så alternativet Formula eller CellData bör fungera tillsammans med alternativet DefinedNames (Formula\\|DefinedNames eller CellData\\|DefinedNames) för de flesta scenarier.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Läs in hyperlänkar

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Läs in sammanslagna celler

### NONE {#NONE}
```
public static final int NONE
```


Läs in inget för bladdata

**Remarks**

OBS: Denna medlem är nu föråldrad och vänligen använd Structure istället. Denna egenskap kommer att tas bort 12 månader senare från och med december 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


Läs in OleObjects

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Läs in bilder

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Läs in pivottabeller

### REVISION {#REVISION}
```
public static final int REVISION
```


Läs in revisionsloggar

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Läs in inställningar för arbetsbok och arbetsblad

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Läs in former

**Remarks**

OBS: Denna medlem är nu föråldrad och vänligen använd Drawing istället. Denna egenskap kommer att tas bort 12 månader senare från och med november 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Läs in all data för arbetsblad, såsom celldata, inställningar, objekt, ...etc.

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Läs in inställningar för arbetsblad

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Läs in strukturen för arbetsboken

### STYLE {#STYLE}
```
public static final int STYLE
```


Läs in stilar för cellformatering

### TABLE {#TABLE}
```
public static final int TABLE
```


Läs in tabeller

### VBA {#VBA}
```
public static final int VBA
```


Läs in VBA-projekt

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


Läs in XmlMap

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

