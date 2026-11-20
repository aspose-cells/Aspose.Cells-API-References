---
title: "Top10"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrive la regola di formattazione condizionale Top10."
type: docs
url: /it/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Descrivi la regola di formattazione condizionale Top10. Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia dei primi N o degli ultimi N, come specificato.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = CellArea.createCellArea(0, 0, 10, 10);
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.TOP_10, OperatorType.NONE, null, null);   
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         Top10 top10 = fc.getTop10();
         //Set the Top N 
         top10.setRank(5);  
         //Saving the Excel file
         workbook.save("output.xls");
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Top10()](#Top10--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Ottiene il valore di "n" in una regola di formattazione condizionale "top/bottom n". |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Restituisce se una regola "top/bottom n" è una regola "bottom n". |
| [isPercent()](#isPercent--) | Restituisce se una regola "top/bottom n" è una regola "top/bottom n percent". |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Imposta se una regola "top/bottom n" è una regola "bottom n". |
| [setPercent(boolean value)](#setPercent-boolean-) | Imposta se una regola "top/bottom n" è una regola "top/bottom n percent". |
| [setRank(int value)](#setRank-int-) | Imposta il valore di "n" in una regola di formattazione condizionale "top/bottom n". |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Top10() {#Top10--}
```
public Top10()
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
### getRank() {#getRank--}
```
public int getRank()
```


Restituisce il valore di "n" in una regola di formattazione condizionale "top/bottom n". Se IsPercent è true, il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Restituisce se una regola "top/bottom n" è una regola "bottom n". Il valore predefinito è false.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Restituisce se una regola "top/bottom n" è una regola "top/bottom n percent". Il valore predefinito è false.

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




### setBottom(boolean value) {#setBottom-boolean-}
```
public void setBottom(boolean value)
```


Imposta se una regola "top/bottom n" è una regola "bottom n". Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Imposta se una regola "top/bottom n" è una regola "top/bottom n percent". Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


Imposta il valore di "n" in una regola di formattazione condizionale "top/bottom n". Se IsPercent è true, il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10.

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

