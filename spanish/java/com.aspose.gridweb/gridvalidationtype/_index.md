---
title: "GridValidationType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el tipo de validación de datos."
type: docs
url: /es/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

Representa el tipo de validación de datos.
## Campos

| Campo | Descripción |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | Tipo de validación de cualquier valor. |
| [BOOLEAN](#BOOLEAN) | VERDADERO o FALSO |
| [CHECK_BOX](#CHECK-BOX) | Muestra la celda como una casilla de verificación. |
| [CUSTOM](#CUSTOM) | Tipo de validación personalizada. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | Tipo de validación personalizada, usando expresión regular. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | Validación con función javascript personalizada. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | Validación con función personalizada del lado del servidor. |
| [DATE](#DATE) | Tipo de validación de fecha. |
| [DATE_TIME](#DATE-TIME) | Fecha y hora (yyyy-MM-dd o yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | Tipo de validación decimal. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | Mostrar lista desplegable. |
| [FREE_LIST](#FREE-LIST) | Tipo de validación de lista libre. |
| [LIST](#LIST) | Tipo de validación de lista. |
| [TEXT_LENGTH](#TEXT-LENGTH) | Tipo de validación de longitud de texto. |
| [TIME](#TIME) | Tipo de validación de hora. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | Tipo de validación de número entero. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```


Tipo de validación de cualquier valor.

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


VERDADERO o FALSO

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


Muestra la celda como una casilla de verificación. Y el valor de la celda es Verdadero o Falso.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Tipo de validación personalizada.

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


Tipo de validación personalizada, usando expresión regular.

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


Validación con función javascript personalizada.

**Remarks**

Utiliza la propiedad ClientValidationFunction para especificar el nombre de la función de validación del cliente. La función debe declararse de la siguiente forma:
function customValicationFunction(source, value)
El parámetro "source" es el objeto celda. El parámetro "value" es el valor de cadena de una celda a comprobar. La función debe devolver true si el valor es válido.

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


Validación con función personalizada del lado del servidor.

**Remarks**

Utiliza la propiedad CustomServerFunction para especificar la validación del lado del servidor. A continuación se muestra el código de ejemplo:
Primero define la clase que implementa GridCustomServerValidation class myservervali : GridCustomServerValidation
...... luego agrega la validación var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); luego establece ClientValidationFunction para manejar la lógica del cliente cuando la validación del servidor falla y devuelve el mensaje gv.ClientValidationFunction = "ValidationErrorClientFunction"; la función del cliente debe declararse así: function ValidationErrorClientFunction(cell,msg) por favor consulta la página de demostración para una referencia detallada

### DATE {#DATE}
```
public static final int DATE
```


Tipo de validación de fecha.

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


Fecha y hora (yyyy-MM-dd o yyyy-MM-dd hh:mm:ss).

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Tipo de validación decimal.

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


Mostrar lista desplegable.

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


Tipo de validación de lista libre.

### LIST {#LIST}
```
public static final int LIST
```


Tipo de validación de lista.

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


Tipo de validación de longitud de texto.

### TIME {#TIME}
```
public static final int TIME
```


Tipo de validación de hora.

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


Tipo de validación de número entero.

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

