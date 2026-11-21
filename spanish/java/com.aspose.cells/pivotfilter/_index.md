---
title: "PivotFilter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un PivotFilter en la colección PivotFilter."
type: docs
url: /es/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Representa un PivotFilter en la colección PivotFilter.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Obtiene el autofiltro del filtro pivot. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Obtiene los valores del filtro numérico. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Obtiene el Orden de Evaluación del filtro pivot. |
| [getFieldIndex()](#getFieldIndex--) | Obtiene el índice del campo origen al que se aplica este filtro pivot. |
| [getFilterCategory()](#getFilterCategory--) | Obtiene la categoría de este filtro. |
| [getFilterType()](#getFilterType--) | Obtiene el tipo de filtro del filtro pivot. |
| [getLabels()](#getLabels--) | Obtiene las etiquetas del filtro de título. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Especifica el índice del campo de cubo de medida. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Obtiene el índice del campo de medida del filtro pivot. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Obtiene el índice del campo de propiedad del miembro del filtro pivot. |
| [getName()](#getName--) | Obtiene el nombre del filtro pivot. |
| [getNumberValues()](#getNumberValues--) | Obtiene los valores del filtro numérico. |
| [getTop10Value()](#getTop10Value--) | Obtiene la configuración de top 10 del filtro. |
| [getUseWholeDay()](#getUseWholeDay--) | Indica si se deben usar días completos en sus criterios de filtrado de fechas. |
| [getValue1()](#getValue1--) | Obtiene el valor de cadena 1 del filtro pivot de etiqueta. |
| [getValue2()](#getValue2--) | Obtiene el valor de cadena 2 del filtro pivot de etiqueta. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Obtiene el índice del campo de valor en la región de valores. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Obtiene el Orden de Evaluación del filtro pivot. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Obtiene el índice del campo de medida del filtro pivot. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Obtiene el índice del campo de propiedad del miembro del filtro pivot. |
| [setName(String value)](#setName-java.lang.String-) | Obtiene el nombre del filtro pivot. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Indica si se deben usar días completos en sus criterios de filtrado de fechas. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Obtiene el valor de cadena 1 del filtro pivot de etiqueta. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Obtiene el valor de cadena 2 del filtro pivot de etiqueta. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Obtiene el índice del campo de valor en la región de valores. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Obtiene el autofiltro del filtro pivot.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método FilterLabel, FilterValue, FilterDate o FilterTop10. Este método será eliminado 12 meses después desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

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


Obtiene los valores del filtro numérico.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Obtiene el Orden de Evaluación del filtro pivot.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Obtiene el índice del campo origen al que se aplica este filtro pivot.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Obtiene la categoría de este filtro.

Ver [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Obtiene el tipo de filtro del filtro pivot.

Ver [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Obtiene las etiquetas del filtro de título.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Especifica el índice del campo del cubo de medida. Esta propiedad se usa solo por filtros en pivotes OLAP y especifica en qué medida debe aplicarse un filtro de valor.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Obtiene el índice del campo de medida del filtro pivot.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotFilter.ValueFieldIndex. Este método será eliminado 12 meses después desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Obtiene el índice del campo de propiedad del miembro del filtro pivot.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del filtro pivot.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Obtiene los valores del filtro numérico.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Obtiene la configuración de top 10 del filtro.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Indica si se deben usar días completos en sus criterios de filtrado de fechas.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Obtiene el valor de cadena 1 del filtro pivot de etiqueta.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Obtiene el valor de cadena 2 del filtro pivot de etiqueta.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Obtiene el índice del campo de valor en la región de valores.

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


Obtiene el Orden de Evaluación del filtro pivot.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Obtiene el índice del campo de medida del filtro pivot.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotFilter.ValueFieldIndex. Este método será eliminado 12 meses después desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Obtiene el índice del campo de propiedad del miembro del filtro pivot.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtiene el nombre del filtro pivot.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Indica si se deben usar días completos en sus criterios de filtrado de fechas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Obtiene el valor de cadena 1 del filtro pivot de etiqueta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Obtiene el valor de cadena 2 del filtro pivot de etiqueta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Obtiene el índice del campo de valor en la región de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

