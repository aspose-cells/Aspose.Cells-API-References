---
title: "PivotShowValuesSetting"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración sobre cómo mostrar valores cuando se utiliza el cálculo ShowDataAs."
type: docs
url: /es/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Representa la configuración sobre cómo mostrar valores cuando se utiliza el cálculo ShowDataAs.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Campos

| Campo | Descripción |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Índice de elemento base especial: use el elemento pivot siguiente. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Índice de elemento base especial: use el elemento pivot anterior. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso. |
| [getBaseFieldName()](#getBaseFieldName--) | Obtiene el título del campo base pivot. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Obtiene el título del elemento pivot en el campo base. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Representa el índice personalizado del elemento pivot en el campo base cuando el cálculo ShowDataAs está en uso. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Representa el tipo del elemento pivot base en el campo base cuando se utiliza el cálculo ShowDataAs. |
| [getCalculationType()](#getCalculationType--) | Representa cómo mostrar los valores de un campo de datos en el informe pivot. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Obtiene cómo mostrar los valores de un campo de datos en el informe pivot. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Representa el índice personalizado del elemento pivot en el campo base cuando el cálculo ShowDataAs está en uso. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Representa el tipo del elemento pivot base en el campo base cuando se utiliza el cálculo ShowDataAs. |
| [setCalculationType(int value)](#setCalculationType-int-) | Representa cómo mostrar los valores de un campo de datos en el informe pivot. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Establece cómo mostrar los valores de un campo de datos en el informe pivot. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Índice de elemento base especial: use el elemento pivot siguiente. Válido para los cálculos "Show Values As"; efectivo en Excel 2010 y versiones posteriores.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Índice de elemento base especial: use el elemento pivot anterior. Válido para los cálculos "Show Values As"; efectivo en Excel 2010 y versiones posteriores.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Obtiene el título del campo base pivot.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Obtiene el título del elemento pivot en el campo base.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Representa el índice personalizado del elemento pivot en el campo base cuando el cálculo ShowDataAs está en uso.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Representa el tipo del elemento pivot base en el campo base cuando se utiliza el cálculo ShowDataAs. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, por favor establezca el atributo PivotField.BaseItemIndex.

Ver [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad PivotShowValuesSetting.BaseItem. Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Representa cómo mostrar los valores de un campo de datos en el informe pivot.

Ver [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad PivotShowValuesSetting.ShowValuesAs. Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Obtiene cómo mostrar los valores de un campo de datos en el informe pivot.

Ver [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Representa el índice personalizado del elemento pivot en el campo base cuando el cálculo ShowDataAs está en uso.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Representa el tipo del elemento pivot base en el campo base cuando se utiliza el cálculo ShowDataAs. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, por favor establezca el atributo PivotField.BaseItemIndex.

Ver [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad PivotShowValuesSetting.BaseItem. Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Representa cómo mostrar los valores de un campo de datos en el informe pivot.

Ver [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad PivotShowValuesSetting.ShowValuesAs. Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Establece cómo mostrar los valores de un campo de datos en el informe pivot.

Ver [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

