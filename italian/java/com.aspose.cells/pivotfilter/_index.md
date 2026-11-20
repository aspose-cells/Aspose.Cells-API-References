---
title: "PivotFilter"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un PivotFilter nella collezione PivotFilter."
type: docs
url: /it/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Rappresenta un PivotFilter nella collezione PivotFilter.

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
 
         //Add top 10 filter
          pivot.getBaseFields().get(0).filterTop10(0, PivotFilterType.COUNT,false,2);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Ottiene l'autofiltro del filtro pivot. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Ottiene i valori del filtro numerico. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Ottiene l'Ordine di valutazione del filtro pivot. |
| [getFieldIndex()](#getFieldIndex--) | Ottiene l'indice del campo sorgente a cui è applicato questo filtro pivot. |
| [getFilterCategory()](#getFilterCategory--) | Ottiene la categoria di questo filtro. |
| [getFilterType()](#getFilterType--) | Ottiene il tipo di filtro del filtro pivot. |
| [getLabels()](#getLabels--) | Ottiene le etichette del filtro di didascalia. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Specifica l'indice del campo cubo di misura. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Ottiene l'indice del campo di misura del filtro pivot. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Ottiene l'indice del campo proprietà del membro del filtro pivot. |
| [getName()](#getName--) | Ottiene il nome del filtro pivot. |
| [getNumberValues()](#getNumberValues--) | Ottiene i valori del filtro numerico. |
| [getTop10Value()](#getTop10Value--) | Ottiene l'impostazione Top 10 del filtro. |
| [getUseWholeDay()](#getUseWholeDay--) | Indica se utilizzare giorni interi nei criteri di filtraggio delle date. |
| [getValue1()](#getValue1--) | Ottiene il valore stringa1 dell'etichetta del filtro pivot. |
| [getValue2()](#getValue2--) | Ottiene il valore stringa2 dell'etichetta del filtro pivot. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Ottiene l'indice del campo valore nella regione dei valori. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Ottiene l'Ordine di valutazione del filtro pivot. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Ottiene l'indice del campo di misura del filtro pivot. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Ottiene l'indice del campo proprietà del membro del filtro pivot. |
| [setName(String value)](#setName-java.lang.String-) | Ottiene il nome del filtro pivot. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Indica se utilizzare giorni interi nei criteri di filtraggio delle date. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Ottiene il valore stringa1 dell'etichetta del filtro pivot. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Ottiene il valore stringa2 dell'etichetta del filtro pivot. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Ottiene l'indice del campo valore nella regione dei valori. |
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
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Ottiene l'autofiltro del filtro pivot.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare i metodi FilterLabel, FilterValue, FilterDate o FilterTop10. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValues() {#getDateTimeValues--}
```
public DateTime[] getDateTimeValues()
```


Ottiene i valori del filtro numerico.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Ottiene l'Ordine di valutazione del filtro pivot.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Ottiene l'indice del campo sorgente a cui è applicato questo filtro pivot.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Ottiene la categoria di questo filtro.

Vedi [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Ottiene il tipo di filtro del filtro pivot.

Vedi [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Ottiene le etichette del filtro di didascalia.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Specifica l'indice del campo del cubo di misura. Questa proprietà è utilizzata solo dai filtri nei pivot OLAP e specifica su quale misura deve essere applicato un filtro di valore.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Ottiene l'indice del campo di misura del filtro pivot.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotFilter.ValueFieldIndex. Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Ottiene l'indice del campo proprietà del membro del filtro pivot.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del filtro pivot.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Ottiene i valori del filtro numerico.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Ottiene l'impostazione Top 10 del filtro.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Indica se utilizzare giorni interi nei criteri di filtraggio delle date.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Ottiene il valore stringa1 dell'etichetta del filtro pivot.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Ottiene il valore stringa2 dell'etichetta del filtro pivot.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Ottiene l'indice del campo valore nella regione dei valori.

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




### setEvaluationOrder(int value) {#setEvaluationOrder-int-}
```
public void setEvaluationOrder(int value)
```


Ottiene l'Ordine di valutazione del filtro pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Ottiene l'indice del campo di misura del filtro pivot.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotFilter.ValueFieldIndex. Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Ottiene l'indice del campo proprietà del membro del filtro pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ottiene il nome del filtro pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Indica se utilizzare giorni interi nei criteri di filtraggio delle date.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Ottiene il valore stringa1 dell'etichetta del filtro pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Ottiene il valore stringa2 dell'etichetta del filtro pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Ottiene l'indice del campo valore nella regione dei valori.

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

