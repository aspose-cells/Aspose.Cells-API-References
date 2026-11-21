---
title: "PivotFilter"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett PivotFilter i PivotFilter-samlingen."
type: docs
url: /sv/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Representerar ett PivotFilter i PivotFilter-samlingen.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Hämtar autofiltret för pivottfiltret. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Hämtar värdena för nummerfiltret. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Hämtar utvärderingsordningen för pivotfiltret. |
| [getFieldIndex()](#getFieldIndex--) | Hämtar indexet för källfältet som detta pivotfilter tillämpas på. |
| [getFilterCategory()](#getFilterCategory--) | Hämtar kategorin för detta filter. |
| [getFilterType()](#getFilterType--) | Hämtar filtertypen för pivotfiltret. |
| [getLabels()](#getLabels--) | Hämtar etiketter för rubrikfiltret. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Anger indexet för måttkubfältet. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Hämtar måttfältets index för pivotfiltret. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Hämtar medlemsegenskapsfältets index för pivotfiltret. |
| [getName()](#getName--) | Hämtar namnet på pivotfiltret. |
| [getNumberValues()](#getNumberValues--) | Hämtar värdena för nummerfiltret. |
| [getTop10Value()](#getTop10Value--) | Hämtar top 10‑inställningen för filtret. |
| [getUseWholeDay()](#getUseWholeDay--) | Anger om hela dagar ska användas i dess datumfiltreringskriterier. |
| [getValue1()](#getValue1--) | Hämtar strängvärdet value1 för etikettpivotfiltret. |
| [getValue2()](#getValue2--) | Hämtar strängvärdet value2 för etikettpivotfiltret. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Hämtar indexet för värdefältet i värdeområdet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Hämtar utvärderingsordningen för pivotfiltret. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Hämtar måttfältets index för pivotfiltret. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Hämtar medlemsegenskapsfältets index för pivotfiltret. |
| [setName(String value)](#setName-java.lang.String-) | Hämtar namnet på pivotfiltret. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Anger om hela dagar ska användas i dess datumfiltreringskriterier. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Hämtar strängvärdet value1 för etikettpivotfiltret. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Hämtar strängvärdet value2 för etikettpivotfiltret. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Hämtar indexet för värdefältet i värdeområdet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Hämtar autofiltret för pivottfiltret.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället FilterLabel, FilterValue, FilterDate eller FilterTop10‑metoden. Denna metod kommer att tas bort 12 månader senare, från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar värdena för nummerfiltret.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Hämtar utvärderingsordningen för pivotfiltret.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Hämtar indexet för källfältet som detta pivotfilter tillämpas på.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Hämtar kategorin för detta filter.

Se [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Hämtar filtertypen för pivotfiltret.

Se [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Hämtar etiketter för rubrikfiltret.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Anger indexet för måttkubfältet. Denna egenskap används endast av filter i OLAP‑pivot och anger på vilket mått ett värdefilter ska tillämpas.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Hämtar måttfältets index för pivotfiltret.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotFilter.ValueFieldIndex. Denna metod kommer att tas bort 12 månader senare, från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Hämtar medlemsegenskapsfältets index för pivotfiltret.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på pivotfiltret.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Hämtar värdena för nummerfiltret.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Hämtar top 10‑inställningen för filtret.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Anger om hela dagar ska användas i dess datumfiltreringskriterier.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Hämtar strängvärdet value1 för etikettpivotfiltret.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Hämtar strängvärdet value2 för etikettpivotfiltret.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Hämtar indexet för värdefältet i värdeområdet.

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


Hämtar utvärderingsordningen för pivotfiltret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Hämtar måttfältets index för pivotfiltret.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotFilter.ValueFieldIndex. Denna metod kommer att tas bort 12 månader senare, från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Hämtar medlemsegenskapsfältets index för pivotfiltret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Hämtar namnet på pivotfiltret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Anger om hela dagar ska användas i dess datumfiltreringskriterier.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Hämtar strängvärdet value1 för etikettpivotfiltret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Hämtar strängvärdet value2 för etikettpivotfiltret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Hämtar indexet för värdefältet i värdeområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

