---
title: "PivotFieldSortSetting"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'impostazione per l'ordinamento dei campi pivot."
type: docs
url: /it/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Rappresenta l'impostazione per l'ordinamento dei campi pivot.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Sort by the first data field ascending.
         rowField.sortBy(SortOrder.ASCENDING, 0, null);
 
         //Gets sort settings of the pivot field.
         PivotFieldSortSetting sortSetting = rowField.getSortSetting();
         System.out.println(sortSetting.getSortType());
         //do your business
 
         pivot.calculateData();
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Ordina per i valori nella riga o nella colonna. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Rappresenta l'indice del campo per cui è ordinato. |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | Il tipo di riga pivot ordinato per. |
| [getSortBy()](#getSortBy--) | Rappresenta l'indice del campo per cui è ordinato. |
| [getSortType()](#getSortType--) | Rappresenta il [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Indica se verrà applicata un'operazione di ordinamento dati semplice. |
| [isSortByLabels()](#isSortByLabels--) | Indica se ordinare il campo per se stesso o per il campo dati. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Rappresenta l'indice del campo per cui è ordinato. |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Indica se verrà applicata un'operazione di ordinamento dati semplice. |
| [setSortBy(int value)](#setSortBy-int-) | Rappresenta l'indice del campo per cui è ordinato. |
| [setSortType(int value)](#setSortType-int-) | Rappresenta il [SortOrder](../../com.aspose.cells/sortorder). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCell() {#getCell--}
```
public String getCell()
```


Ordina per i valori nella riga o nella colonna.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Rappresenta l'indice del campo per cui è ordinato. -1 indica l'ordinamento del PivotField per le etichette, altri indica l'ordinamento per il campo dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotFieldSortSetting.SortBy. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


Il tipo di riga pivot ordinato per.

Vedi [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

Funziona solo quando questo campo non è ordinato per etichette.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Rappresenta l'indice del campo per cui è ordinato. Un valore di -1 indica l'ordinamento per i valori propri dell'elemento pivot. Quando è maggiore o uguale a zero, rappresenta l'indice del campo dati nella regione dati.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


Rappresenta il [SortOrder](../../com.aspose.cells/sortorder).

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```


Indica se verrà applicata un'operazione di ordinamento dati semplice.

**Remarks**

Il valore predefinito è true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Indica se ordinare il campo per se stesso o per il campo dati.

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




### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Rappresenta l'indice del campo per cui è ordinato. -1 indica l'ordinamento del PivotField per le etichette, altri indica l'ordinamento per il campo dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotFieldSortSetting.SortBy. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Indica se verrà applicata un'operazione di ordinamento dati semplice.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Rappresenta l'indice del campo per cui è ordinato. Un valore di -1 indica l'ordinamento per i valori propri dell'elemento pivot. Quando è maggiore o uguale a zero, rappresenta l'indice del campo dati nella regione dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


Rappresenta il [SortOrder](../../com.aspose.cells/sortorder).

Vedi [SortOrder](../../com.aspose.cells/sortorder).

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

