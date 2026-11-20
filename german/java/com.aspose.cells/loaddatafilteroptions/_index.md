---
title: "LoadDataFilterOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage dar."
type: docs
url: /de/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Stellt die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage dar.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ALL](#ALL) | Alle laden |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Einstellungen für Arbeitsmappe laden |
| [CELL_BLANK](#CELL-BLANK) | Zellen laden, deren Wert leer ist |
| [CELL_BOOL](#CELL-BOOL) | Zellen laden, deren Wert bool ist |
| [CELL_DATA](#CELL-DATA) | Zellendaten laden, einschließlich Werte, Formeln und Formatierung |
| [CELL_ERROR](#CELL-ERROR) | Lade Zellen, deren Wert ein Fehler ist |
| [CELL_NUMERIC](#CELL-NUMERIC) | Lade Zellen, deren Wert numerisch ist (einschließlich Datum/Zeit) |
| [CELL_STRING](#CELL-STRING) | Lade Zellen, deren Wert ein String ist |
| [CELL_VALUE](#CELL-VALUE) | Lade nur Zellenwerte (alle Werttypen) |
| [CHART](#CHART) | Lade Diagramme |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Lade bedingte Formatierung |
| [DATA_VALIDATION](#DATA-VALIDATION) | Lade Datenvalidierungen |
| [DEFINED_NAMES](#DEFINED-NAMES) | Lade definierte Namensobjekte |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Lade Dokumenteigenschaften |
| [DRAWING](#DRAWING) | Zeichenobjekte (einschließlich Diagramm, Bild, OleObject und alle anderen Zeichenobjekte) |
| [FORMULA](#FORMULA) | Lade Zellformeln. |
| [HYPERLINKS](#HYPERLINKS) | Lade Hyperlinks |
| [MERGED_AREA](#MERGED-AREA) | Lade zusammengeführte Zellen |
| [NONE](#NONE) | Lade nichts für Blattdaten |
| [OLE_OBJECT](#OLE-OBJECT) | Lade OleObjects |
| [PICTURE](#PICTURE) | Lade Bilder |
| [PIVOT_TABLE](#PIVOT-TABLE) | Lade Pivot-Tabellen |
| [REVISION](#REVISION) | Lade Revisionsprotokolle |
| [SETTINGS](#SETTINGS) | Lade Einstellungen für Arbeitsmappe und Arbeitsblatt |
| [SHAPE](#SHAPE) | Lade Formen |
| [SHEET_DATA](#SHEET-DATA) | Lade alle Daten des Arbeitsblatts, wie Zellen­daten, Einstellungen, Objekte, … usw. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Lade Einstellungen für das Arbeitsblatt |
| [STRUCTURE](#STRUCTURE) | Lade Struktur der Arbeitsmappe |
| [STYLE](#STYLE) | Lade Stile für Zellformatierung |
| [TABLE](#TABLE) | Lade Tabellen |
| [VBA](#VBA) | VBA-Projekte laden |
| [XML_MAP](#XML-MAP) | XmlMap laden |
## Methoden

| Methode | Beschreibung |
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


Alle laden

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Einstellungen für Arbeitsmappe laden

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Zellen laden, deren Wert leer ist

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Zellen laden, deren Wert bool ist

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Zellendaten laden, einschließlich Werte, Formeln und Formatierung

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Lade Zellen, deren Wert ein Fehler ist

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Lade Zellen, deren Wert numerisch ist (einschließlich Datum/Zeit)

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Lade Zellen, deren Wert ein String ist

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Lade nur Zellenwerte (alle Werttypen)

### CHART {#CHART}
```
public static final int CHART
```


Lade Diagramme

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Lade bedingte Formatierung

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Lade Datenvalidierungen

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Lade definierte Namensobjekte

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Lade Dokumenteigenschaften

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Zeichenobjekte (einschließlich Diagramm, Bild, OleObject und alle anderen Zeichenobjekte)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Lade Zellformeln.

**Remarks**

Im Allgemeinen müssen definierte Namensobjekte(DefinedNames) ebenfalls geladen werden, wenn Formeln geladen werden, da sie von Formeln referenziert werden können. Daher sollte die Option Formula oder CellData zusammen mit der Option DefinedNames (Formula\|DefinedNames oder CellData\|DefinedNames) in den meisten Szenarien funktionieren.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Lade Hyperlinks

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Lade zusammengeführte Zellen

### NONE {#NONE}
```
public static final int NONE
```


Lade nichts für Blattdaten

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet und bitte verwenden Sie stattdessen Structure. Diese Eigenschaft wird 12 Monate später, seit Dezember 2017, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


Lade OleObjects

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Lade Bilder

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Lade Pivot-Tabellen

### REVISION {#REVISION}
```
public static final int REVISION
```


Lade Revisionsprotokolle

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Lade Einstellungen für Arbeitsmappe und Arbeitsblatt

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Lade Formen

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet und bitte verwenden Sie stattdessen Drawing. Diese Eigenschaft wird 12 Monate später, seit November 2019, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Lade alle Daten des Arbeitsblatts, wie Zellen­daten, Einstellungen, Objekte, … usw.

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Lade Einstellungen für das Arbeitsblatt

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Lade Struktur der Arbeitsmappe

### STYLE {#STYLE}
```
public static final int STYLE
```


Lade Stile für Zellformatierung

### TABLE {#TABLE}
```
public static final int TABLE
```


Lade Tabellen

### VBA {#VBA}
```
public static final int VBA
```


VBA-Projekte laden

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


XmlMap laden

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

