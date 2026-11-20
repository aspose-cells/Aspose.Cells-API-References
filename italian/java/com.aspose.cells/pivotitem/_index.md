---
title: "PivotItem"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un elemento in un report PivotField."
type: docs
url: /it/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

Rappresenta un elemento in un report PivotField.

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
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Campi

| Campo | Descrizione |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Indice sentinella di selezione di tutti gli elementi della pagina (0x7FFD, non è un indice valido) |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Restituisce il valore data/ora dell'elemento pivot. Se il valore è null, restituisce DateTime.MinValue |
| [getDoubleValue()](#getDoubleValue--) | Restituisce il valore double dell'elemento pivot. Se il valore è null o non è un numero, restituisce 0 |
| [getFormula()](#getFormula--) | Restituisce la formula di questo elemento calcolato. |
| [getIndex()](#getIndex--) | Restituisce l'indice dell'elemento pivot nel campo cache. |
| [getName()](#getName--) | Restituisce il nome dell'elemento pivot. |
| [getPosition()](#getPosition--) | Specificare l'indice di questo elemento in tutti i PivotItems del campo. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Specificare l'indice di posizione nei PivotItems sotto lo stesso nodo padre. |
| [getStringValue()](#getStringValue--) | Restituisce il valore stringa dell'elemento pivot. Se il valore è null, restituisce "". |
| [getValue()](#getValue--) | Restituisce il valore dell'elemento pivot. |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Imposta se l'elemento pivot è nascosto. |
| [isCalculatedItem()](#isCalculatedItem--) | Indica se questo elemento pivot è un elemento di formula calcolata. |
| [isDetailHidden()](#isDetailHidden--) | Restituisce se il dettaglio di questo elemento pivot è nascosto. |
| [isFormula()](#isFormula--) | Indica se questo elemento pivot è un elemento di formula calcolata. |
| [isHidden()](#isHidden--) | Restituisce se l'elemento pivot è nascosto. |
| [isHideDetail()](#isHideDetail--) | Restituisce se l'elemento pivot nasconde il dettaglio. |
| [isMissing()](#isMissing--) | Indica se l'elemento è stato rimosso dalla fonte dati. |
| [move(int offset)](#move-int-) | Sposta l'elemento su o giù nel campo pivot |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Sposta l'elemento su o giù |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Imposta se il dettaglio di questo elemento pivot è nascosto. |
| [setFormula(boolean value)](#setFormula-boolean-) | Indica se questo elemento pivot è un elemento di formula calcolata. |
| [setHidden(boolean value)](#setHidden-boolean-) | Imposta se l'elemento pivot è nascosto. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Imposta se l'elemento pivot nasconde il dettaglio. |
| [setIndex(int value)](#setIndex-int-) | Restituisce l'indice dell'elemento pivot nel campo cache. |
| [setName(String value)](#setName-java.lang.String-) | Restituisce il nome dell'elemento pivot. |
| [setPosition(int value)](#setPosition-int-) | Specificare l'indice di questo elemento in tutti i PivotItems del campo. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Specificare l'indice di posizione nei PivotItems sotto lo stesso nodo padre. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Indice sentinella di selezione di tutti gli elementi della pagina (0x7FFD, non è un indice valido)

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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Restituisce il valore data/ora dell'elemento pivot. Se il valore è null, restituisce DateTime.MinValue

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Restituisce il valore double dell'elemento pivot. Se il valore è null o non è un numero, restituisce 0

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Restituisce la formula di questo elemento calcolato. Funziona solo quando questo elemento è un elemento calcolato.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Restituisce l'indice dell'elemento pivot nel campo cache.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.Position. Questo metodo sarà rimosso 6 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Restituisce il nome dell'elemento pivot.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Specificare l'indice di questo elemento in tutti i PivotItems del campo.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Specificare l'indice di posizione nei PivotItems sotto lo stesso nodo padre.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.MoveItem(PivotFieldType, string[],bool,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Restituisce il valore stringa dell'elemento pivot. Se il valore è null, restituisce "".

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Restituisce il valore dell'elemento pivot.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Imposta se l'elemento pivot è nascosto.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Aspose.Cells.Pivot.PivotItem.IsHidden. Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2012. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Indica se questo elemento pivot è un elemento di formula calcolata.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Restituisce se il dettaglio di questo elemento pivot è nascosto.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indica se questo elemento pivot è un elemento di formula calcolata.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.IsCalculatedItem. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Restituisce se l'elemento pivot è nascosto.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Restituisce se l'elemento pivot nasconde il dettaglio.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.IsDetailHidden. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Indica se l'elemento è stato rimosso dalla fonte dati.

**Remarks**

True indica che questo valore è stato rimosso dalla fonte dati.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Sposta l'elemento su o giù nel campo pivot

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| offset | int | Il numero di spostamenti verso l'alto o verso il basso. Sposta l'elemento verso l'alto se questo è inferiore a zero; sposta l'elemento verso il basso se è superiore a zero. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Sposta l'elemento su o giù

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.MoveItem(PivotFieldType, string[],bool,int) o il metodo PivotItem.Move(int). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| offset | int | Il numero di spostamenti verso l'alto o verso il basso. Sposta l'elemento verso l'alto se questo è inferiore a zero; sposta l'elemento verso il basso se è superiore a zero. |
| isSameParent | boolean | Specificare se l'operazione di spostamento è nello stesso nodo padre o meno |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Imposta se il dettaglio di questo elemento pivot è nascosto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Indica se questo elemento pivot è un elemento di formula calcolata.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.IsCalculatedItem. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Imposta se l'elemento pivot è nascosto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Imposta se l'elemento pivot nasconde il dettaglio.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.IsDetailHidden. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Restituisce l'indice dell'elemento pivot nel campo cache.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.Position. Questo metodo sarà rimosso 6 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Restituisce il nome dell'elemento pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Specificare l'indice di questo elemento in tutti i PivotItems del campo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Specificare l'indice di posizione nei PivotItems sotto lo stesso nodo padre.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.MoveItem(PivotFieldType, string[],bool,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

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

