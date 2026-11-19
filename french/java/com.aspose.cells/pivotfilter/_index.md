---
title: "PivotFilter"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un PivotFilter dans la collection PivotFilter."
type: docs
url: /fr/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Représente un PivotFilter dans la collection PivotFilter.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Obtient l'autofilter du filtre pivot. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Obtient les valeurs du filtre numérique. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Obtient l'ordre d'évaluation du filtre pivot. |
| [getFieldIndex()](#getFieldIndex--) | Obtient l'index du champ source auquel ce filtre pivot est appliqué. |
| [getFilterCategory()](#getFilterCategory--) | Obtient la catégorie de ce filtre. |
| [getFilterType()](#getFilterType--) | Obtient le type de filtre du filtre pivot. |
| [getLabels()](#getLabels--) | Obtient les libellés du filtre de légende. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Spécifie l'index du champ cube de mesure. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Obtient l'index du champ de mesure du filtre pivot. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Obtient l'index du champ de propriété du membre du filtre pivot. |
| [getName()](#getName--) | Obtient le nom du filtre pivot. |
| [getNumberValues()](#getNumberValues--) | Obtient les valeurs du filtre numérique. |
| [getTop10Value()](#getTop10Value--) | Obtient le paramètre top 10 du filtre. |
| [getUseWholeDay()](#getUseWholeDay--) | Indique s'il faut utiliser des jours complets dans les critères de filtrage de date. |
| [getValue1()](#getValue1--) | Obtient la chaîne value1 du filtre pivot d'étiquette. |
| [getValue2()](#getValue2--) | Obtient la chaîne value2 du filtre pivot d'étiquette. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Obtient l'index du champ de valeur dans la région des valeurs. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Obtient l'ordre d'évaluation du filtre pivot. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Obtient l'index du champ de mesure du filtre pivot. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Obtient l'index du champ de propriété du membre du filtre pivot. |
| [setName(String value)](#setName-java.lang.String-) | Obtient le nom du filtre pivot. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Indique s'il faut utiliser des jours complets dans les critères de filtrage de date. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Obtient la chaîne value1 du filtre pivot d'étiquette. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Obtient la chaîne value2 du filtre pivot d'étiquette. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Obtient l'index du champ de valeur dans la région des valeurs. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Obtient l'autofilter du filtre pivot.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode FilterLabel, FilterValue, FilterDate ou FilterTop10. Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

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


Obtient les valeurs du filtre numérique.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Obtient l'ordre d'évaluation du filtre pivot.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Obtient l'index du champ source auquel ce filtre pivot est appliqué.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Obtient la catégorie de ce filtre.

Voir [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Obtient le type de filtre du filtre pivot.

Voir [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Obtient les libellés du filtre de légende.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Spécifie l'index du champ cube de mesure. Cette propriété n'est utilisée que par les filtres dans les tableaux croisés OLAP et indique sur quelle mesure un filtre de valeur doit s'appliquer.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Obtient l'index du champ de mesure du filtre pivot.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotFilter.ValueFieldIndex. Cette méthode sera supprimée 12 mois après, depuis novembre 2024. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Obtient l'index du champ de propriété du membre du filtre pivot.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom du filtre pivot.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Obtient les valeurs du filtre numérique.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Obtient le paramètre top 10 du filtre.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Indique s'il faut utiliser des jours complets dans les critères de filtrage de date.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Obtient la chaîne value1 du filtre pivot d'étiquette.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Obtient la chaîne value2 du filtre pivot d'étiquette.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Obtient l'index du champ de valeur dans la région des valeurs.

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


Obtient l'ordre d'évaluation du filtre pivot.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Obtient l'index du champ de mesure du filtre pivot.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotFilter.ValueFieldIndex. Cette méthode sera supprimée 12 mois après, depuis novembre 2024. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Obtient l'index du champ de propriété du membre du filtre pivot.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtient le nom du filtre pivot.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Indique s'il faut utiliser des jours complets dans les critères de filtrage de date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Obtient la chaîne value1 du filtre pivot d'étiquette.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Obtient la chaîne value2 du filtre pivot d'étiquette.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Obtient l'index du champ de valeur dans la région des valeurs.

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

