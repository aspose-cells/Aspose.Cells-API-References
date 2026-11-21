---
title: "Validación"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa data validation.settings."
type: docs
url: /es/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

Representa data validation.settings.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Aplica la validación al área. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Aplica la validación al área. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Aplica la validación a las áreas dadas. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Copiar validación. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Representa el estilo de alerta de validación. |
| [getAreas()](#getAreas--) | Obtiene todas las [CellArea](../../com.aspose.cells/cellarea) que contienen la configuración de validación de datos. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Representa el mensaje de error de validación de datos. |
| [getErrorTitle()](#getErrorTitle--) | Representa el título del cuadro de diálogo de error de validación de datos. |
| [getFormula1()](#getFormula1--) | Representa el valor o expresión asociado con la validación de datos. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Obtiene el valor o expresión asociado con esta validación. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Obtiene el valor o expresión asociado con esta validación para una celda específica. |
| [getFormula2()](#getFormula2--) | Representa el valor o expresión asociado con la validación de datos. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Obtiene el valor o expresión asociado con esta validación. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Obtiene el valor o expresión asociado con esta validación para una celda específica. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Indica si se permiten valores en blanco por la validación de datos del rango. |
| [getInCellDropDown()](#getInCellDropDown--) | Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables. |
| [getInputMessage()](#getInputMessage--) | Representa el mensaje de entrada de la validación de datos. |
| [getInputTitle()](#getInputTitle--) | Representa el título del cuadro de diálogo de entrada de la validación de datos. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Obtiene el valor de la lista de validación para la celda especificada. |
| [getOperator()](#getOperator--) | Representa el operador de la validación de datos. |
| [getShowError()](#getShowError--) | Indica si el mensaje de error de la validación de datos se mostrará siempre que el usuario introduzca datos no válidos. |
| [getShowInput()](#getShowInput--) | Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación. |
| [getType()](#getType--) | Representa el tipo de validación de datos. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Obtiene el valor de la validación en la celda específica. |
| [getValue1()](#getValue1--) | Representa el primer valor asociado a la validación de datos. |
| [getValue2()](#getValue2--) | Representa el segundo valor asociado a la validación de datos. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Elimina la configuración de validación en la celda. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Elimina la configuración de validación en el rango. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Elimina esta validación de las áreas especificadas. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Representa el estilo de alerta de validación. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Representa el mensaje de error de validación de datos. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Representa el título del cuadro de diálogo de error de validación de datos. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Representa el valor o expresión asociado con la validación de datos. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Establece el valor o expresión asociado a esta validación. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Representa el valor o expresión asociado con la validación de datos. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Establece el valor o expresión asociado a esta validación. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Indica si se permiten valores en blanco por la validación de datos del rango. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Representa el mensaje de entrada de la validación de datos. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Representa el título del cuadro de diálogo de entrada de la validación de datos. |
| [setOperator(int value)](#setOperator-int-) | Representa el operador de la validación de datos. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indica si el mensaje de error de la validación de datos se mostrará siempre que el usuario introduzca datos no válidos. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación. |
| [setType(int value)](#setType-int-) | Representa el tipo de validación de datos. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Representa el primer valor asociado a la validación de datos. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Representa el segundo valor asociado a la validación de datos. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Aplica la validación al área.

**Remarks**

Equivale a usar [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) con comprobación de intersección y borde.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | El área. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Aplica la validación al área.

**Remarks**

En este método, eliminaremos todas las validaciones antiguas en el área especificada. Para la zona superior‑izquierda de los rangos aplicados de Validation, primero su StartRow es el más pequeño, segundo su StartColumn es el más pequeño de esas áreas que comparten el mismo StartRow más bajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | El área. |
| checkIntersection | boolean | Indica si se debe comprobar la intersección del área dada con las áreas de validaciones existentes. Si una validación se ha aplicado en el área dada (o en parte de ella), entonces la validación existente debe eliminarse primero del área dada. De lo contrario, la generación de Validations puede corromperse. Si el usuario está seguro de que el área añadida no intersecta con ninguna área existente, este parámetro puede establecerse en false por consideraciones de rendimiento. |
| checkEdge | boolean | Indica si se debe comprobar el borde de las áreas aplicadas de esta validación. La configuración interna de Validation depende de la zona superior‑izquierda de sus rangos aplicados, por lo que si el área dada llega a ser la nueva zona superior‑izquierda de los rangos aplicados, la configuración interna debe modificarse y reconstruirse; de lo contrario, pueden producirse resultados inesperados. Si el usuario está seguro de que el área añadida no es la zona superior‑izquierda, este parámetro puede establecerse en false por consideraciones de rendimiento. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Aplica la validación a las áreas dadas.

**Remarks**

En este método, eliminaremos todas las validaciones antiguas en el área especificada. Para la zona superior‑izquierda de los rangos aplicados de Validation, primero su StartRow es el más pequeño, segundo su StartColumn es el más pequeño de esas áreas que comparten el mismo StartRow más bajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Las áreas. |
| checkIntersection | boolean | Indica si se debe comprobar la intersección del área dada con las áreas de validaciones existentes. Si una validación se ha aplicado en el área dada (o en parte de ella), entonces la validación existente debe eliminarse primero del área dada. De lo contrario, la generación de Validations puede corromperse. Si el usuario está seguro de que todas las áreas añadidas no intersectan con ninguna área existente, este parámetro puede establecerse en false por consideraciones de rendimiento. |
| checkEdge | boolean | Indica si se debe comprobar el borde de las áreas aplicadas de esta validación. La configuración interna de Validation depende de la zona superior‑izquierda de sus rangos aplicados, por lo que si una de las áreas dadas llega a ser la nueva zona superior‑izquierda de los rangos aplicados, la configuración interna debe modificarse y reconstruirse; de lo contrario, pueden producirse resultados inesperados. Si el usuario está seguro de que ninguna de esas áreas añadidas es la zona superior‑izquierda, este parámetro puede establecerse en false por consideraciones de rendimiento. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Copiar validación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | La validación de origen. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | La opción de copia. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Representa el estilo de alerta de validación.

Ver [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Obtiene todas las [CellArea](../../com.aspose.cells/cellarea) que contienen la configuración de validación de datos.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Representa el mensaje de error de validación de datos.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Representa el título del cuadro de diálogo de error de validación de datos.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Representa el valor o expresión asociado con la validación de datos.

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Obtiene el valor o expresión asociado con esta validación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - El valor o expresión asociado con esta validación.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtiene el valor o expresión asociado con esta validación para una celda específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.String - El valor o expresión asociado con esta validación.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Representa el valor o expresión asociado con la validación de datos.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Obtiene el valor o expresión asociado con esta validación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - El valor o expresión asociado con esta validación.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtiene el valor o expresión asociado con esta validación para una celda específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.String - El valor o expresión asociado con esta validación.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Indica si se permiten valores en blanco por la validación de datos del rango.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Representa el mensaje de entrada de la validación de datos.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Representa el título del cuadro de diálogo de entrada de la validación de datos.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Obtiene el valor de la lista de validación para la celda especificada.

**Remarks**

Solo para validaciones cuyo tipo es List y se ha aplicado a la celda dada, de lo contrario se devolverá null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

**Returns:**
java.lang.Object - El valor para generar la lista de esta validación para la celda especificada. Si la lista hace referencia a un rango, entonces el valor devuelto será un objeto [ReferredArea](../../com.aspose.cells/referredarea); de lo contrario, el valor devuelto puede ser null, object[] o un objeto simple.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Representa el operador de la validación de datos.

Ver [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Indica si el mensaje de error de la validación de datos se mostrará siempre que el usuario introduzca datos no válidos.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Representa el tipo de validación de datos.

Ver [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Obtiene el valor de la validación en la celda específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |
| isValue1 | boolean | Indica si se está obteniendo el primer valor. |

**Returns:**
java.lang.Object - 
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Representa el primer valor asociado a la validación de datos.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Representa el segundo valor asociado a la validación de datos.

**Returns:**
java.lang.Object
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Elimina la configuración de validación en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Elimina la configuración de validación en el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | las áreas donde se deben eliminar estas configuraciones de validación. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Elimina esta validación de las áreas especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | las áreas donde se deben eliminar estas configuraciones de validación. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Representa el estilo de alerta de validación.

Ver [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Representa el mensaje de error de validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Representa el título del cuadro de diálogo de error de validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Representa el valor o expresión asociado con la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Establece el valor o expresión asociado a esta validación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | El valor o expresión asociado con esta condición de formato. |
| isR1C1 | boolean | Si la fórmula es una fórmula R1C1. |
| isLocal | boolean | Si la fórmula está formateada según la configuración regional. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Representa el valor o expresión asociado con la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Establece el valor o expresión asociado a esta validación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | El valor o expresión asociado con esta condición de formato. |
| isR1C1 | boolean | Si la fórmula es una fórmula R1C1. |
| isLocal | boolean | Si la fórmula está formateada según la configuración regional. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Indica si se permiten valores en blanco por la validación de datos del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Representa el mensaje de entrada de la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Representa el título del cuadro de diálogo de entrada de la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Representa el operador de la validación de datos.

Ver [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Indica si el mensaje de error de la validación de datos se mostrará siempre que el usuario introduzca datos no válidos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Representa el tipo de validación de datos.

Ver [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Representa el primer valor asociado a la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Representa el segundo valor asociado a la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

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

