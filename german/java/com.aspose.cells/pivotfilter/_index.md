---
title: "PivotFilter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen PivotFilter in der PivotFilter‑Sammlung dar."
type: docs
url: /de/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Stellt einen PivotFilter in der PivotFilter‑Sammlung dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Liefert den Autofilter des Pivotfilters. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Liefert die Werte des Zahlenfilters. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Liefert die Auswertungsreihenfolge des Pivotfilters. |
| [getFieldIndex()](#getFieldIndex--) | Liefert den Index des Quellfeldes, auf das dieser Pivotfilter angewendet wird. |
| [getFilterCategory()](#getFilterCategory--) | Liefert die Kategorie dieses Filters. |
| [getFilterType()](#getFilterType--) | Liefert den Filtertyp des Pivotfilters. |
| [getLabels()](#getLabels--) | Liefert die Bezeichnungen des Beschriftungsfilters. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Gibt den Index des Messwürfel-Feldes an. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Liefert den Index des Messfeldes des Pivotfilters. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Liefert den Index des Mitgliedseigenschaftsfeldes des Pivotfilters. |
| [getName()](#getName--) | Liefert den Namen des Pivotfilters. |
| [getNumberValues()](#getNumberValues--) | Liefert die Werte des Zahlenfilters. |
| [getTop10Value()](#getTop10Value--) | Liefert die Top‑10‑Einstellung des Filters. |
| [getUseWholeDay()](#getUseWholeDay--) | Gibt an, ob bei den Datumsfilterkriterien ganze Tage verwendet werden sollen. |
| [getValue1()](#getValue1--) | Liefert den Zeichenkettenwert value1 des Label-Pivotfilters. |
| [getValue2()](#getValue2--) | Liefert den Zeichenkettenwert value2 des Label-Pivotfilters. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Liefert den Index des Wertefelds im Wertebereich. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Liefert die Auswertungsreihenfolge des Pivotfilters. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Liefert den Index des Messfeldes des Pivotfilters. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Liefert den Index des Mitgliedseigenschaftsfeldes des Pivotfilters. |
| [setName(String value)](#setName-java.lang.String-) | Liefert den Namen des Pivotfilters. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Gibt an, ob bei den Datumsfilterkriterien ganze Tage verwendet werden sollen. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Liefert den Zeichenkettenwert value1 des Label-Pivotfilters. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Liefert den Zeichenkettenwert value2 des Label-Pivotfilters. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Liefert den Index des Wertefelds im Wertebereich. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Liefert den Autofilter des Pivotfilters.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode FilterLabel, FilterValue, FilterDate oder FilterTop10. Diese Methode wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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


Liefert die Werte des Zahlenfilters.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Liefert die Auswertungsreihenfolge des Pivotfilters.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Liefert den Index des Quellfeldes, auf das dieser Pivotfilter angewendet wird.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Liefert die Kategorie dieses Filters.

Siehe [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Liefert den Filtertyp des Pivotfilters.

Siehe [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Liefert die Bezeichnungen des Beschriftungsfilters.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Gibt den Index des Measure-Cube-Felds an. Diese Eigenschaft wird nur von Filtern in OLAP-Pivot-Tabellen verwendet und gibt an, auf welches Measure ein Wertefilter angewendet werden soll.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Liefert den Index des Messfeldes des Pivotfilters.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PivotFilter.ValueFieldIndex. Diese Methode wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Liefert den Index des Mitgliedseigenschaftsfeldes des Pivotfilters.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen des Pivotfilters.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Liefert die Werte des Zahlenfilters.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Liefert die Top‑10‑Einstellung des Filters.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Gibt an, ob bei den Datumsfilterkriterien ganze Tage verwendet werden sollen.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Liefert den Zeichenkettenwert value1 des Label-Pivotfilters.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Liefert den Zeichenkettenwert value2 des Label-Pivotfilters.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Liefert den Index des Wertefelds im Wertebereich.

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


Liefert die Auswertungsreihenfolge des Pivotfilters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Liefert den Index des Messfeldes des Pivotfilters.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PivotFilter.ValueFieldIndex. Diese Methode wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Liefert den Index des Mitgliedseigenschaftsfeldes des Pivotfilters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Liefert den Namen des Pivotfilters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Gibt an, ob bei den Datumsfilterkriterien ganze Tage verwendet werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Liefert den Zeichenkettenwert value1 des Label-Pivotfilters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Liefert den Zeichenkettenwert value2 des Label-Pivotfilters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Liefert den Index des Wertefelds im Wertebereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

