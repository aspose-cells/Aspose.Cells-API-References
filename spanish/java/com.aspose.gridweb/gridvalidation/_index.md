---
title: "GridValidation"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa data validation.settings."
type: docs
url: /es/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Representa data validation.settings.
## Campos

| Campo | Descripción |
| --- | --- |
| [ServerValidation](#ServerValidation) | Obtiene o establece el nombre de la función JavaScript de validación del lado del servidor. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | agrega la configuración de validación en la celda. |
| [addACell(String cellname)](#addACell-java.lang.String-) | agrega la configuración de validación en la celda. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Aplica la validación al área. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Representa una colección de [GridCellArea](../../com.aspose.gridweb/gridcellarea) que contiene la configuración de validación de datos. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Obtiene el nombre de la función JavaScript de validación del cliente. |
| [getErrorMessage()](#getErrorMessage--) | Representa el mensaje de error de validación de datos. |
| [getErrorTitle()](#getErrorTitle--) | Representa el título del cuadro de diálogo de error de validación de datos. |
| [getFormula1()](#getFormula1--) | Representa el valor o expresión asociado con la validación de datos. |
| [getFormula2()](#getFormula2--) | Representa el valor o expresión asociado con la segunda parte de la validación de datos. |
| [getInputMessage()](#getInputMessage--) | Representa el mensaje de error de validación de datos. |
| [getInputTitle()](#getInputTitle--) | Representa el título del cuadro de diálogo de entrada de la validación de datos. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Obtiene el valor de la lista de validación para la celda especificada. |
| [getOperator()](#getOperator--) | Representa el operador de la validación de datos. |
| [getRegEx()](#getRegEx--) | Obtiene la cadena de expresión regular. |
| [getShowError()](#getShowError--) | Indica si el mensaje de error de la validación de datos se mostrará siempre que el usuario introduzca datos no válidos. |
| [getShowInput()](#getShowInput--) | Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación. |
| [getValidationType()](#getValidationType--) | Obtiene el tipo de validación. |
| [getValue1()](#getValue1--) | Representa el valor asociado con la validación de datos. |
| [getValueList()](#getValueList--) | Obtiene el objeto de lista de valores. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Obtiene si el valor de la celda es obligatorio. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Elimina la configuración de validación en la celda. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Elimina la configuración de validación en el rango. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Establece el nombre de la función JavaScript de validación del cliente. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Representa el mensaje de error de validación de datos. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Representa el título del cuadro de diálogo de error de validación de datos. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Representa el valor o expresión asociado con la validación de datos. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Representa el valor o expresión asociado con la segunda parte de la validación de datos. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Representa el mensaje de error de validación de datos. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Representa el título del cuadro de diálogo de entrada de la validación de datos. |
| [setOperator(int value)](#setOperator-int-) | Representa el operador de la validación de datos. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Establece la cadena de expresión regular. |
| [setRequired(boolean value)](#setRequired-boolean-) | Establece si el valor de la celda es obligatorio. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indica si el mensaje de error de la validación de datos se mostrará siempre que el usuario introduzca datos no válidos. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación. |
| [setValidationType(int value)](#setValidationType-int-) | Establece el tipo de validación. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Establece el objeto de lista de valores. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Obtiene o establece el nombre de la función JavaScript de validación del lado del servidor.

**Remarks**

Utiliza la propiedad GridCustomServerValidation para especificar la validación del lado del servidor.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


agrega la configuración de validación en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila. |
| columna | int | El índice de columna. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


agrega la configuración de validación en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellname | java.lang.String | nombre de celda. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Aplica la validación al área.

**Remarks**

En este método, eliminaremos todas las validaciones antiguas en esta área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El área. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Representa una colección de [GridCellArea](../../com.aspose.gridweb/gridcellarea) que contiene la configuración de validación de datos.

**Remarks**

Las validaciones antiguas en el área no se eliminarán si se añaden directamente a esta lista.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


Obtiene el nombre de la función JavaScript de validación del cliente.

**Remarks**

Utiliza la propiedad ClientValidationFunction para especificar el nombre de la función de validación del cliente. La función debe declararse de la siguiente forma:
function customValicationFunction(source, value)
El parámetro "source" es el objeto celda. El parámetro "value" es el valor de cadena de una celda a comprobar. La función debe devolver true si el valor es válido.

**Returns:**
java.lang.String
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
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Representa el valor o expresión asociado con la segunda parte de la validación de datos.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Representa el mensaje de error de validación de datos.

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
java.lang.Object - El valor para producir la lista de esta validación para la celda especificada. Si la lista hace referencia a un rango, entonces el valor devuelto será un objeto ReferredArea; de lo contrario, el valor devuelto puede ser null, object[] o un objeto simple.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Representa el operador de la validación de datos.

Ver [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Obtiene la cadena de expresión regular.

**Returns:**
java.lang.String
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
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Obtiene el tipo de validación.

Ver [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Representa el valor asociado con la validación de datos.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Obtiene el objeto de lista de valores.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


Obtiene si el valor de la celda es obligatorio.

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

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Elimina la configuración de validación en el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El rango que contiene la configuración de validación de datos. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


Establece el nombre de la función JavaScript de validación del cliente.

**Remarks**

Utiliza la propiedad ClientValidationFunction para especificar el nombre de la función de validación del cliente. La función debe declararse de la siguiente forma:
function customValicationFunction(source, value)
El parámetro "source" es el objeto celda. El parámetro "value" es el valor de cadena de una celda a comprobar. La función debe devolver true si el valor es válido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Representa el valor o expresión asociado con la segunda parte de la validación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Representa el mensaje de error de validación de datos.

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

Ver [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Establece la cadena de expresión regular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Establece si el valor de la celda es obligatorio.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Establece el tipo de validación.

Ver [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Establece el objeto de lista de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.ArrayList<java.lang.String> |  |

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

