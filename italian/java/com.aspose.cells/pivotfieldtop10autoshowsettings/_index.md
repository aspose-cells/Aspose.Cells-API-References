---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni Top 10 AutoShow per un campo pivot."
type: docs
url: /it/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Rappresenta le impostazioni Top 10 AutoShow per un campo pivot.

**Remarks**

In xls: implementazione dei filtri top 10 in Xls tramite Top 10 AutoShow. Nei file ooxml: il formato ooxml sottostante supporta Top10 AutoShow, ma l'interfaccia utente di Excel 2007 e versioni successive fornisce l'accesso solo tramite filtro Top10. Se la compatibilità XLS non è necessaria, si consiglia di utilizzare invece il filtro Top10.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Specifica l'indice del campo dati per la classifica AutoShow. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Indica se è stato applicato un filtro "Top 10 AutoShow" a questo campo. |
| [isTop()](#isTop--) | Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indica se è stato applicato un filtro "Top 10 AutoShow" a questo campo. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato. |
| [setRankBy(int value)](#setRankBy-int-) | Specifica l'indice del campo dati per la classifica AutoShow. |
| [setTop(boolean value)](#setTop-boolean-) | Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Specifica l'indice del campo dati per la classifica AutoShow. Rappresenta l'indice del campo auto show. -1 indica il PivotField stesso. Deve essere l'indice dei campi dati.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indica se è stato applicato un filtro "Top 10 AutoShow" a questo campo.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indica se è stato applicato un filtro "Top 10 AutoShow" a questo campo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Specifica l'indice del campo dati per la classifica AutoShow. Rappresenta l'indice del campo auto show. -1 indica il PivotField stesso. Deve essere l'indice dei campi dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

