---
title: "LoadDataFilterOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per filtrare i dati durante il caricamento della cartella di lavoro da un modello."
type: docs
url: /it/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Rappresenta le opzioni per filtrare i dati durante il caricamento della cartella di lavoro da un modello.
## Campi

| Campo | Descrizione |
| --- | --- |
| [ALL](#ALL) | Carica tutto |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Carica impostazioni per la cartella di lavoro |
| [CELL_BLANK](#CELL-BLANK) | Carica celle il cui valore è vuoto |
| [CELL_BOOL](#CELL-BOOL) | Carica celle il cui valore è booleano |
| [CELL_DATA](#CELL-DATA) | Carica i dati delle celle includendo valori, formule e formattazione |
| [CELL_ERROR](#CELL-ERROR) | Carica celle il cui valore è errore |
| [CELL_NUMERIC](#CELL-NUMERIC) | Carica le celle il cui valore è numerico(inclusi data/ora) |
| [CELL_STRING](#CELL-STRING) | Carica le celle il cui valore è stringa |
| [CELL_VALUE](#CELL-VALUE) | Carica solo il valore delle celle(tutti i tipi di valore) |
| [CHART](#CHART) | Carica i grafici |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Carica la formattazione condizionale |
| [DATA_VALIDATION](#DATA-VALIDATION) | Carica le convalide dei dati |
| [DEFINED_NAMES](#DEFINED-NAMES) | Carica gli oggetti Nome definiti |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Carica le proprietà del documento |
| [DRAWING](#DRAWING) | Oggetti di disegno(inclusi Chart, Picture, OleObject e tutti gli altri oggetti di disegno) |
| [FORMULA](#FORMULA) | Carica le formule delle celle. |
| [HYPERLINKS](#HYPERLINKS) | Carica i collegamenti ipertestuali |
| [MERGED_AREA](#MERGED-AREA) | Carica le celle unite |
| [NONE](#NONE) | Non caricare nulla per i dati del foglio |
| [OLE_OBJECT](#OLE-OBJECT) | Carica OleObjects |
| [PICTURE](#PICTURE) | Carica le immagini |
| [PIVOT_TABLE](#PIVOT-TABLE) | Carica le tabelle pivot |
| [REVISION](#REVISION) | Carica i registri delle revisioni |
| [SETTINGS](#SETTINGS) | Carica le impostazioni per la cartella di lavoro e il foglio di lavoro |
| [SHAPE](#SHAPE) | Carica le forme |
| [SHEET_DATA](#SHEET-DATA) | Carica tutti i dati del foglio di lavoro, come dati delle celle, impostazioni, oggetti, ...ecc. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Carica le impostazioni per il foglio di lavoro |
| [STRUCTURE](#STRUCTURE) | Carica la struttura della cartella di lavoro |
| [STYLE](#STYLE) | Carica gli stili per la formattazione delle celle |
| [TABLE](#TABLE) | Carica le tabelle |
| [VBA](#VBA) | Carica i progetti VBA |
| [XML_MAP](#XML-MAP) | Carica XmlMap |
## Metodi

| Metodo | Descrizione |
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


Carica tutto

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Carica impostazioni per la cartella di lavoro

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Carica celle il cui valore è vuoto

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Carica celle il cui valore è booleano

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Carica i dati delle celle includendo valori, formule e formattazione

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Carica celle il cui valore è errore

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Carica le celle il cui valore è numerico(inclusi data/ora)

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Carica le celle il cui valore è stringa

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Carica solo il valore delle celle(tutti i tipi di valore)

### CHART {#CHART}
```
public static final int CHART
```


Carica i grafici

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Carica la formattazione condizionale

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Carica le convalide dei dati

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Carica gli oggetti Nome definiti

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Carica le proprietà del documento

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Oggetti di disegno(inclusi Chart, Picture, OleObject e tutti gli altri oggetti di disegno)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Carica le formule delle celle.

**Remarks**

In genere gli oggetti Name definiti (DefinedNames) devono anche essere caricati durante il caricamento delle formule perché potrebbero essere referenziati dalle formule. Quindi l'opzione Formula o CellData dovrebbe funzionare insieme all'opzione DefinedNames (Formula\|DefinedNames o CellData\|DefinedNames) per la maggior parte degli scenari.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Carica i collegamenti ipertestuali

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Carica le celle unite

### NONE {#NONE}
```
public static final int NONE
```


Non caricare nulla per i dati del foglio

**Remarks**

NOTA: Questo membro è ora obsoleto e si prega di utilizzare Structure invece. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


Carica OleObjects

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Carica le immagini

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Carica le tabelle pivot

### REVISION {#REVISION}
```
public static final int REVISION
```


Carica i registri delle revisioni

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Carica le impostazioni per la cartella di lavoro e il foglio di lavoro

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Carica le forme

**Remarks**

NOTA: Questo membro è ora obsoleto e si prega di utilizzare Drawing invece. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2019. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Carica tutti i dati del foglio di lavoro, come dati delle celle, impostazioni, oggetti, ...ecc.

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Carica le impostazioni per il foglio di lavoro

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Carica la struttura della cartella di lavoro

### STYLE {#STYLE}
```
public static final int STYLE
```


Carica gli stili per la formattazione delle celle

### TABLE {#TABLE}
```
public static final int TABLE
```


Carica le tabelle

### VBA {#VBA}
```
public static final int VBA
```


Carica i progetti VBA

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


Carica XmlMap

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

