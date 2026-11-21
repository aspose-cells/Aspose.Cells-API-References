---
title: "PivotItem"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un elemento en un informe de PivotField."
type: docs
url: /es/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

Representa un elemento en un informe de PivotField.

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
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Campos

| Campo | Descripción |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Índice centinela de seleccionar todo de los elementos de página (0x7FFD, no es un índice válido) |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Obtiene el valor de fecha y hora del elemento pivot. Si el valor es null, devolverá DateTime.MinValue. |
| [getDoubleValue()](#getDoubleValue--) | Obtiene el valor double del elemento pivot. Si el valor es null o no es un número, devolverá 0. |
| [getFormula()](#getFormula--) | Obtiene la fórmula de este elemento calculado. |
| [getIndex()](#getIndex--) | Obtiene el índice del elemento pivot en el campo de caché. |
| [getName()](#getName--) | Obtiene el nombre del elemento pivot. |
| [getPosition()](#getPosition--) | Especificando el índice de este elemento en todos los PivotItems del campo. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Especificando el índice de posición en los PivotItems bajo el mismo nodo padre. |
| [getStringValue()](#getStringValue--) | Obtiene el valor de cadena del elemento pivot. Si el valor es nulo, devolverá "" |
| [getValue()](#getValue--) | Obtiene el valor del elemento pivot |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Establece si el elemento pivot está oculto. |
| [isCalculatedItem()](#isCalculatedItem--) | Indica si este elemento pivot es un elemento de fórmula calculada. |
| [isDetailHidden()](#isDetailHidden--) | Obtiene si el detalle de este elemento pivot está oculto. |
| [isFormula()](#isFormula--) | Indica si este elemento pivot es un elemento de fórmula calculada. |
| [isHidden()](#isHidden--) | Obtiene si el elemento pivot está oculto. |
| [isHideDetail()](#isHideDetail--) | Obtiene si el elemento pivot oculta el detalle. |
| [isMissing()](#isMissing--) | Indica si el elemento fue eliminado de la fuente de datos. |
| [move(int offset)](#move-int-) | Mueve el elemento hacia arriba o abajo en el campo pivot |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Mueve el elemento hacia arriba o abajo |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Establece si el detalle de este elemento pivot está oculto. |
| [setFormula(boolean value)](#setFormula-boolean-) | Indica si este elemento pivot es un elemento de fórmula calculada. |
| [setHidden(boolean value)](#setHidden-boolean-) | Establece si el elemento pivot está oculto. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Establece si el elemento pivot oculta el detalle. |
| [setIndex(int value)](#setIndex-int-) | Obtiene el índice del elemento pivot en el campo de caché. |
| [setName(String value)](#setName-java.lang.String-) | Obtiene el nombre del elemento pivot. |
| [setPosition(int value)](#setPosition-int-) | Especificando el índice de este elemento en todos los PivotItems del campo. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Especificando el índice de posición en los PivotItems bajo el mismo nodo padre. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Índice centinela de seleccionar todo de los elementos de página (0x7FFD, no es un índice válido)

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Obtiene el valor de fecha y hora del elemento pivot. Si el valor es null, devolverá DateTime.MinValue.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Obtiene el valor double del elemento pivot. Si el valor es null o no es un número, devolverá 0.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtiene la fórmula de este elemento calculado. Solo funciona cuando este elemento es un elemento calculado.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice del elemento pivot en el campo de caché.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.Position. Este método será eliminado 6 meses después, desde agosto de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del elemento pivot.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Especificando el índice de este elemento en todos los PivotItems del campo.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Especificando el índice de posición en los PivotItems bajo el mismo nodo padre.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.MoveItem(PivotFieldType, string[],bool,int). Este método será eliminado 12 meses después, desde noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtiene el valor de cadena del elemento pivot. Si el valor es nulo, devolverá ""

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor del elemento pivot

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Establece si el elemento pivot está oculto.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Aspose.Cells.Pivot.PivotItem.IsHidden. Esta propiedad será eliminada 12 meses después, desde enero de 2012. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Indica si este elemento pivot es un elemento de fórmula calculada.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Obtiene si el detalle de este elemento pivot está oculto.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indica si este elemento pivot es un elemento de fórmula calculada.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.IsCalculatedItem. Esta propiedad será eliminada 12 meses después, desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Obtiene si el elemento pivot está oculto.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Obtiene si el elemento pivot oculta el detalle.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.IsDetailHidden. Esta propiedad será eliminada 12 meses después, desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Indica si el elemento fue eliminado de la fuente de datos.

**Remarks**

True indica que este valor ha sido eliminado de la fuente de datos.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Mueve el elemento hacia arriba o abajo en el campo pivot

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desplazamiento | int | El número de movimientos hacia arriba o abajo. Mueva el elemento hacia arriba si esto es menor que cero; mueva el elemento hacia abajo si esto es mayor que cero. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Mueve el elemento hacia arriba o abajo

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.MoveItem(PivotFieldType, string[],bool,int) o el método PivotItem.Move(int). Este método será eliminado 12 meses después, desde noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desplazamiento | int | El número de movimientos hacia arriba o abajo. Mueva el elemento hacia arriba si esto es menor que cero; mueva el elemento hacia abajo si esto es mayor que cero. |
| isSameParent | boolean | Especificando si la operación de movimiento está en el mismo nodo padre o no |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Establece si el detalle de este elemento pivot está oculto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Indica si este elemento pivot es un elemento de fórmula calculada.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.IsCalculatedItem. Esta propiedad será eliminada 12 meses después, desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Establece si el elemento pivot está oculto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Establece si el elemento pivot oculta el detalle.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.IsDetailHidden. Esta propiedad será eliminada 12 meses después, desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Obtiene el índice del elemento pivot en el campo de caché.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.Position. Este método será eliminado 6 meses después, desde agosto de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtiene el nombre del elemento pivot.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Especificando el índice de este elemento en todos los PivotItems del campo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Especificando el índice de posición en los PivotItems bajo el mismo nodo padre.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.MoveItem(PivotFieldType, string[],bool,int). Este método será eliminado 12 meses después, desde noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

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

