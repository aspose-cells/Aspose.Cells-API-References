---
title: "PivotArea"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Presenta l'area selezionata della tabella pivot."
type: docs
url: /it/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Presenta l'area selezionata della tabella pivot.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Presenta l'area selezionata della Tabella pivot. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Ottiene la regione della Tabella pivot a cui si applica questa regola. |
| [getCellAreas()](#getCellAreas--) | Ottiene le aree di celle di questa area pivot. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Ottiene tutti i filtri per questa Area pivot. |
| [getOnlyData()](#getOnlyData--) | Indica se sono selezionati solo i valori dei dati (nell'area dati della visualizzazione) per una selezione di elementi e non includono le etichette degli elementi. |
| [getOnlyLabel()](#getOnlyLabel--) | Indica se sono selezionate solo le etichette dei dati per una selezione di elementi. |
| [getRuleType()](#getRuleType--) | Ottiene il tipo di regola di selezione. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Indica se il totale generale della colonna è incluso. |
| [isOutline()](#isOutline--) | Indica se la regola si riferisce a un'area in modalità contorno. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Indica se il totale generale della riga è incluso. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Seleziona l'area con i filtri. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Seleziona un campo nella regione come area. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Seleziona un campo nella regione come area. |
| [setAxisType(int value)](#setAxisType-int-) | Imposta la regione della Tabella pivot a cui si applica questa regola. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Indica se il totale generale della colonna è incluso. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Indica se sono selezionati solo i valori dei dati (nell'area dati della visualizzazione) per una selezione di elementi e non includono le etichette degli elementi. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Indica se sono selezionate solo le etichette dei dati per una selezione di elementi. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indica se la regola si riferisce a un'area in modalità contorno. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Indica se il totale generale della riga è incluso. |
| [setRuleType(int value)](#setRuleType-int-) | Imposta il tipo di regola di selezione. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


Presenta l'area selezionata della Tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Ottiene la regione della Tabella pivot a cui si applica questa regola.

Vedi [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Ottiene le aree di celle di questa area pivot.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```


Ottiene tutti i filtri per questa Area pivot.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Indica se sono selezionati solo i valori dei dati (nell'area dati della visualizzazione) per una selezione di elementi e non includono le etichette degli elementi.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Indica se sono selezionate solo le etichette dei dati per una selezione di elementi.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Ottiene il tipo di regola di selezione.

Vedi [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```


Indica se il totale generale della colonna è incluso.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Indica se la regola si riferisce a un'area in modalità contorno.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Indica se il totale generale della riga è incluso.

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




### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```


Seleziona l'area con i filtri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La regione della PivotTable a cui si applica questa regola. |
| fieldPosition | int | Posizione del campo all'interno dell'asse a cui si applica questa regola. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Specifica cosa può essere selezionato in una PivotTable durante una selezione strutturata. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Seleziona un campo nella regione come area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di regione. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Il campo pivot. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Seleziona un campo nella regione come area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di regione. |
| fieldName | java.lang.String | Il nome del campo pivot. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Imposta la regione della Tabella pivot a cui si applica questa regola.

Vedi [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Indica se il totale generale della colonna è incluso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Indica se sono selezionati solo i valori dei dati (nell'area dati della visualizzazione) per una selezione di elementi e non includono le etichette degli elementi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Indica se sono selezionate solo le etichette dei dati per una selezione di elementi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Indica se la regola si riferisce a un'area in modalità contorno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Indica se il totale generale della riga è incluso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Imposta il tipo di regola di selezione.

Vedi [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

