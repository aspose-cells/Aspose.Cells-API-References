---
title: "PivotFieldGroupOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni per le impostazioni di raggruppamento del campo pivot."
type: docs
url: /it/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Opzioni per le impostazioni di raggruppamento del campo pivot.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Ottiene gli elementi di gruppo discreti. |
| [getEndDate()](#getEndDate--) | Ottiene il valore finale dell'intervallo di raggruppamento. |
| [getEndNumber()](#getEndNumber--) | Ottiene il valore finale dell'intervallo di raggruppamento. |
| [getGroupType()](#getGroupType--) | Ottiene il tipo di raggruppamento per il campo pivot. |
| [getGroupTypes()](#getGroupTypes--) | Ottiene il tipo di raggruppamento per il campo pivot. |
| [getInterval()](#getInterval--) | Ottiene la dimensione dell'intervallo per ogni gruppo. |
| [getNewPivotField()](#getNewPivotField--) | Ottiene un valore che indica se devono essere creati nuovi campi pivot dopo il raggruppamento. |
| [getStartDate()](#getStartDate--) | Ottiene il valore iniziale dell'intervallo di raggruppamento. |
| [getStartNumber()](#getStartNumber--) | Ottiene il valore iniziale dell'intervallo di raggruppamento. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Ottiene un valore che indica se il valore finale è determinato automaticamente. |
| [isAutoStart()](#isAutoStart--) | Ottiene un valore che indica se il valore iniziale è determinato automaticamente. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Imposta un valore che indica se il valore finale è determinato automaticamente. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Imposta un valore che indica se il valore iniziale è determinato automaticamente. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Imposta gli elementi di gruppo discreti. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Imposta il valore finale dell'intervallo di raggruppamento. |
| [setEndNumber(double value)](#setEndNumber-double-) | Imposta il valore finale dell'intervallo di raggruppamento. |
| [setGroupType(int value)](#setGroupType-int-) | Imposta il tipo di raggruppamento per il campo pivot. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Imposta il tipo di raggruppamento per il campo pivot. |
| [setInterval(double value)](#setInterval-double-) | Imposta la dimensione dell'intervallo per ogni gruppo. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Imposta un valore che indica se devono essere creati nuovi campi pivot dopo il raggruppamento. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Imposta il valore iniziale dell'intervallo di raggruppamento. |
| [setStartNumber(double value)](#setStartNumber-double-) | Imposta il valore iniziale dell'intervallo di raggruppamento. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
```


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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Ottiene gli elementi di gruppo discreti.

**Remarks**

Se questa proprietà è impostata,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Ottiene il valore finale dell'intervallo di raggruppamento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Ottiene il valore finale dell'intervallo di raggruppamento.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Restituisce il tipo di raggruppamento per il campo pivot. Solo per il raggruppamento del campo pivot data/ora.

Vedi [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Ottiene il tipo di raggruppamento per il campo pivot.

Vedi [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

L'ordine in questa proprietà sarà ignorato. Quando si specificano più tipi di gruppo, i campi di gruppo di base saranno inseriti in ordine crescente e il campo di gruppo verrà mostrato nella regione riga/colonna in ordine decrescente (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Ottiene la dimensione dell'intervallo per ogni gruppo.

**Remarks**

Solo per il gruppo di numeri e giorni.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Ottiene un valore che indica se devono essere creati nuovi campi pivot dopo il raggruppamento.

**Remarks**

Se non impostato esplicitamente, il valore predefinito è false per il raggruppamento numerico e true per il raggruppamento data/ora, true per il gruppo discreto. Funziona solo per il primo nuovo campo pivot di gruppo del campo base.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Ottiene il valore iniziale dell'intervallo di raggruppamento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Ottiene il valore iniziale dell'intervallo di raggruppamento.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Ottiene un valore che indica se il valore finale è determinato automaticamente.

**Remarks**

Se [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) o [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) è impostato, questa proprietà sarà false.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Ottiene un valore che indica se il valore iniziale è determinato automaticamente.

**Remarks**

Se [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) o [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) è impostato, questa proprietà sarà false.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Imposta un valore che indica se il valore finale è determinato automaticamente.

**Remarks**

Se [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) o [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) è impostato, questa proprietà sarà false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Imposta un valore che indica se il valore iniziale è determinato automaticamente.

**Remarks**

Se [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) o [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) è impostato, questa proprietà sarà false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Imposta gli elementi di gruppo discreti.

**Remarks**

Se questa proprietà è impostata,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Imposta il valore finale dell'intervallo di raggruppamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Imposta il valore finale dell'intervallo di raggruppamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Imposta il tipo di raggruppamento per il campo pivot. Solo per il raggruppamento del campo pivot data/ora.

Vedi [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Imposta il tipo di raggruppamento per il campo pivot.

Vedi [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

L'ordine in questa proprietà sarà ignorato. Quando si specificano più tipi di gruppo, i campi di gruppo di base saranno inseriti in ordine crescente e il campo di gruppo verrà mostrato nella regione riga/colonna in ordine decrescente (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Imposta la dimensione dell'intervallo per ogni gruppo.

**Remarks**

Solo per il gruppo di numeri e giorni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Imposta un valore che indica se devono essere creati nuovi campi pivot dopo il raggruppamento.

**Remarks**

Se non impostato esplicitamente, il valore predefinito è false per il raggruppamento numerico e true per il raggruppamento data/ora, true per il gruppo discreto. Funziona solo per il primo nuovo campo pivot di gruppo del campo base.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Imposta il valore iniziale dell'intervallo di raggruppamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Imposta il valore iniziale dell'intervallo di raggruppamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

