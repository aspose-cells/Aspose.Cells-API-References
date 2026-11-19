---
title: "Top10"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Décrit la règle de mise en forme conditionnelle Top10."
type: docs
url: /fr/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Décrivez la règle de mise en forme conditionnelle Top10. Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans la tranche supérieure N ou inférieure N, selon spécification.

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
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Top10()](#Top10--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Obtient la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Obtient si une règle "top/bottom n" est une règle "bottom n". |
| [isPercent()](#isPercent--) | Obtient si une règle "top/bottom n" est une règle "top/bottom n percent". |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Définit si une règle "top/bottom n" est une règle "bottom n". |
| [setPercent(boolean value)](#setPercent-boolean-) | Définit si une règle "top/bottom n" est une règle "top/bottom n percent". |
| [setRank(int value)](#setRank-int-) | Définit la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". |
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
| Paramètre | Type | Description |
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


Obtient la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". Si IsPercent est vrai, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. La valeur par défaut est 10.

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


Obtient si une règle "top/bottom n" est une règle "bottom n". Valeur par défaut est false.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Obtient si une règle "top/bottom n" est une règle "top/bottom n percent". Valeur par défaut est false.

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


Définit si une règle "top/bottom n" est une règle "bottom n". Valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Définit si une règle "top/bottom n" est une règle "top/bottom n percent". Valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


Définit la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". Si IsPercent est vrai, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. La valeur par défaut est 10.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

