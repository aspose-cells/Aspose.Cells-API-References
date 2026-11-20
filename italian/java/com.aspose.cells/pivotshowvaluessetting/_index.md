---
title: "PivotShowValuesSetting"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni relative alla visualizzazione dei valori quando il calcolo ShowDataAs è in uso."
type: docs
url: /it/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Rappresenta le impostazioni relative alla visualizzazione dei valori quando il calcolo ShowDataAs è in uso.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Campi

| Campo | Descrizione |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Indice speciale dell'elemento base: utilizza l'elemento pivot successivo. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Indice speciale dell'elemento base: utilizza l'elemento pivot precedente. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso. |
| [getBaseFieldName()](#getBaseFieldName--) | Ottiene la didascalia del campo base pivot. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Ottiene la didascalia dell'elemento pivot nel campo base. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Rappresenta l'indice personalizzato dell'elemento pivot nel campo base quando il calcolo ShowDataAs è in uso. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Rappresenta il tipo dell'elemento pivot di base nel campo di base quando è in uso il calcolo ShowDataAs. |
| [getCalculationType()](#getCalculationType--) | Rappresenta come visualizzare i valori di un campo dati nel report pivot. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Ottiene come visualizzare i valori di un campo dati nel report pivot. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Rappresenta l'indice personalizzato dell'elemento pivot nel campo base quando il calcolo ShowDataAs è in uso. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Rappresenta il tipo dell'elemento pivot di base nel campo di base quando è in uso il calcolo ShowDataAs. |
| [setCalculationType(int value)](#setCalculationType-int-) | Rappresenta come visualizzare i valori di un campo dati nel report pivot. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Imposta come visualizzare i valori di un campo dati nel report pivot. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Indice speciale dell'elemento di base: utilizza l'elemento pivot successivo. Valido per i calcoli \"Show Values As\"; efficace in Excel 2010 e versioni successive.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Indice speciale dell'elemento di base: utilizza l'elemento pivot precedente. Valido per i calcoli \"Show Values As\"; efficace in Excel 2010 e versioni successive.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Ottiene la didascalia del campo base pivot.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Ottiene la didascalia dell'elemento pivot nel campo base.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Rappresenta l'indice personalizzato dell'elemento pivot nel campo base quando il calcolo ShowDataAs è in uso.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Rappresenta il tipo dell'elemento pivot di base nel campo di base quando è in uso il calcolo ShowDataAs. Poiché PivotItemPosition.Custom è solo in lettura, se è necessario impostare PivotItemPosition.Custom, impostare l'attributo PivotField.BaseItemIndex.

Vedi [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotShowValuesSetting.BaseItem. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per eventuali disagi subiti.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Rappresenta come visualizzare i valori di un campo dati nel report pivot.

Vedi [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotShowValuesSetting.ShowValuesAs. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per eventuali disagi subiti.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Ottiene come visualizzare i valori di un campo dati nel report pivot.

Vedi [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

**Returns:**
int
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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Rappresenta l'indice personalizzato dell'elemento pivot nel campo base quando il calcolo ShowDataAs è in uso.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Rappresenta il tipo dell'elemento pivot di base nel campo di base quando è in uso il calcolo ShowDataAs. Poiché PivotItemPosition.Custom è solo in lettura, se è necessario impostare PivotItemPosition.Custom, impostare l'attributo PivotField.BaseItemIndex.

Vedi [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotShowValuesSetting.BaseItem. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per eventuali disagi subiti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Rappresenta come visualizzare i valori di un campo dati nel report pivot.

Vedi [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotShowValuesSetting.ShowValuesAs. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per eventuali disagi subiti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Imposta come visualizzare i valori di un campo dati nel report pivot.

Vedi [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

