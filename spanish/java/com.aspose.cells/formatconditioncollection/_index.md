---
title: "FormatConditionCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el formato condicional."
type: docs
url: /es/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Representa el formato condicional. Las FormatConditions pueden contener hasta tres formatos condicionales.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Agrega una condición de formato y el rango de celdas afectado a las FormatConditions. Las FormatConditions pueden contener hasta tres formatos condicionales. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Agrega un rango de celdas con formato condicional. |
| [addCondition(int type)](#addCondition-int-) | Agregar una condición de formato. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Agrega una condición de formato. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene la condición de formato por índice. |
| [getCellArea(int index)](#getCellArea-int-) | Obtiene el rango de celdas con formato condicional por índice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el recuento de las condiciones. |
| [getRangeCount()](#getRangeCount--) | Obtiene el recuento de los rangos con formato condicional. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Elimina el rango de celdas con formato condicional por índice. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Eliminar el formato condicional en el rango. |
| [removeCondition(int index)](#removeCondition-int-) | Elimina la condición de formato por índice. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Agrega una condición de formato y el rango de celdas afectado a los FormatConditions. Los FormatConditions pueden contener hasta tres formatos condicionales. No se permiten referencias a otras hojas en las fórmulas de formato condicional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Rango de celdas con formato condicional. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Tipo de formato condicional. Puede ser uno de los miembros de FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Operador de comparación. Puede ser uno de los miembros de OperatorType. |
| formula1 | java.lang.String | El valor o expresión asociado con el formato condicional. |
| formula2 | java.lang.String | El valor o expresión asociado con el formato condicional |

**Returns:**
int[] - [0]:Índice del objeto de condición de formato;[1] Índice del rango de celdas afectado.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Agrega un rango de celdas con formato condicional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Rango de celdas con formato condicional. |

**Returns:**
int - Índice del rango de celdas con formato condicional.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Agregar una condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Tipo de condición de formato. |

**Returns:**
int - Índice del objeto de condición de formato;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Agrega una condición de formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). El tipo de condición de formato. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). El tipo de operador |
| formula1 | java.lang.String | El valor o expresión asociado con el formato condicional. Si el valor de entrada comienza con '=', se tomará como una fórmula. De lo contrario se tomará como un valor simple (texto, número, booleano). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\\"=...\\"". |
| formula2 | java.lang.String | El valor o expresión asociado con el formato condicional. El formato de entrada es el mismo que formula1 |

**Returns:**
int - Índice del objeto de condición de formato;
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


Obtiene la condición de formato por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice de la condición de formato a devolver. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Obtiene el rango de celdas con formato condicional por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del rango de celdas con formato condicional. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el recuento de las condiciones.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Obtiene el recuento de los rangos con formato condicional.

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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Elimina el rango de celdas con formato condicional por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del rango de celdas con formato condicional que se eliminará. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Eliminar el formato condicional en el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La startRow del rango. |
| startColumn | int | La startColumn del rango. |
| totalRows | int | El número de filas del rango. |
| totalColumns | int | El número de columnas del rango. |

**Returns:**
boolean - Devuelve TRUE, esta FormatCondtionCollection debe ser eliminada.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Elimina la condición de formato por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de la condición de formato que se eliminará. |

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

