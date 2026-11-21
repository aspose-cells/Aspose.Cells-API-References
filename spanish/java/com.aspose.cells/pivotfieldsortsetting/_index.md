---
title: "PivotFieldSortSetting"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración para ordenar los campos dinámicos."
type: docs
url: /es/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Representa la configuración para ordenar los campos dinámicos.

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
 
         //Sort by the first data field ascending.
         rowField.sortBy(SortOrder.ASCENDING, 0, null);
 
         //Gets sort settings of the pivot field.
         PivotFieldSortSetting sortSetting = rowField.getSortSetting();
         System.out.println(sortSetting.getSortType());
         //do your business
 
         pivot.calculateData();
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Ordena por los valores en la fila o columna. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Representa el índice del campo por el cual se ordena |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | El tipo de línea de pivote por el cual se ordena. |
| [getSortBy()](#getSortBy--) | Representa el índice del campo por el cual se ordena. |
| [getSortType()](#getSortType--) | Representa el [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Indica si se aplicará una operación simple de ordenación de datos. |
| [isSortByLabels()](#isSortByLabels--) | Indica si se debe ordenar el campo por sí mismo o por el campo de datos. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Representa el índice del campo por el cual se ordena |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Indica si se aplicará una operación simple de ordenación de datos. |
| [setSortBy(int value)](#setSortBy-int-) | Representa el índice del campo por el cual se ordena. |
| [setSortType(int value)](#setSortType-int-) | Representa el [SortOrder](../../com.aspose.cells/sortorder). |
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
### getCell() {#getCell--}
```
public String getCell()
```


Ordena por los valores en la fila o columna.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Representa el índice del campo por el cual se ordena. -1 significa ordenar el PivotField por las etiquetas, otros significa ordenar por el campo de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotFieldSortSetting.SortBy. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


El tipo de línea de pivote por el cual se ordena.

Ver [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

Solo funciona cuando no se ordena este campo por etiquetas.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Representa el índice del campo por el cual se ordena. Un valor de -1 indica ordenar por los propios valores del elemento de pivote. Cuando es mayor o igual a cero, representa el índice del campo de datos en la región de datos.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


Representa el [SortOrder](../../com.aspose.cells/sortorder).

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```


Indica si se aplicará una operación simple de ordenación de datos.

**Remarks**

El valor predeterminado es true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Indica si se debe ordenar el campo por sí mismo o por el campo de datos.

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




### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Representa el índice del campo por el cual se ordena. -1 significa ordenar el PivotField por las etiquetas, otros significa ordenar por el campo de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotFieldSortSetting.SortBy. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Indica si se aplicará una operación simple de ordenación de datos.

**Remarks**

El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Representa el índice del campo por el cual se ordena. Un valor de -1 indica ordenar por los propios valores del elemento de pivote. Cuando es mayor o igual a cero, representa el índice del campo de datos en la región de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


Representa el [SortOrder](../../com.aspose.cells/sortorder).

Ver [SortOrder](../../com.aspose.cells/sortorder).

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

