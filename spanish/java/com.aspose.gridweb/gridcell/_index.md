---
title: "GridCell"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un objeto de celda."
type: docs
url: /es/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Representa un objeto de celda.
## Métodos

| Método | Descripción |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Indica si esta celda contiene un enlace externo. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Copia datos de una celda origen. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | copia el estilo y establece el estilo para la celda |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Crea un objeto de comentario para una celda. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Crea un objeto de validación para una celda. |
| [equals(Object obj)](#equals-java.lang.Object-) | Comprueba si este objeto se refiere a la misma celda que otro objeto de celda. |
| [getBoolValue()](#getBoolValue--) | Obtiene el valor booleano contenido en la celda. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el número de columna (basado en cero) de la celda. |
| [getComment()](#getComment--) | Obtener el objeto de comentario en esta celda |
| [getDateValue()](#getDateValue--) | Obtiene el valor DateTime contenido en la celda. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Obtiene el valor de cadena formateado de esta celda. |
| [getDoubleValue()](#getDoubleValue--) | Obtiene el valor double contenido en la celda. |
| [getFloatValue()](#getFloatValue--) | Obtiene el valor float contenido en la celda. |
| [getFormula()](#getFormula--) | Obtiene una fórmula del [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Obtiene la cadena HTML que contiene datos y algunos formatos en esta celda. |
| [getIntValue()](#getIntValue--) | Obtiene el valor entero contenido en la celda. |
| [getName()](#getName--) | Obtiene el nombre de la celda. |
| [getRow()](#getRow--) | Obtiene el número de fila (basado en cero) de la celda. |
| [getStringValue()](#getStringValue--) | Obtiene el valor de cadena contenido en la celda. |
| [getStyle()](#getStyle--) | Obtiene una copia del estilo de la celda. establece el estilo para la celda. |
| [getType()](#getType--) | devuelve el tipo de valor de la celda, el significado se puede ver en GridCellValueType.java |
| [getValue()](#getValue--) | Obtiene el valor contenido en esta celda. |
| [getWidthOfValue()](#getWidthOfValue--) | Obtiene el ancho del valor en unidades de píxeles. |
| [hashCode()](#hashCode--) | Sirve como una función hash para un tipo particular. |
| [isErrorValue()](#isErrorValue--) | Comprueba si una fórmula puede evaluar correctamente un resultado. |
| [isFormula()](#isFormula--) | Representa si la celda especificada contiene una fórmula. |
| [isStyleSet()](#isStyleSet--) | Indica si el estilo de la celda está configurado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Inserta un valor booleano en la celda. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Inserta un valor DateTime en la celda. |
| [putValue(double param_double)](#putValue-double-) | Inserta un valor double en la celda. |
| [putValue(int param_int)](#putValue-int-) | Inserta un valor entero en la celda. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Inserta un valor de objeto en la celda. lo mismo que setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | Inserta un valor de cadena en la celda. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Inserta un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Inserta un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Establece el valor de la celda con un valor de cadena y establece el formato de la celda según este valor. |
| [removeComment()](#removeComment--) | Elimina el objeto de comentario de la celda. |
| [removeValidation()](#removeValidation--) | Elimina el objeto de validación de la celda. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Establece bordes (superior, inferior, izquierdo y derecho) para una celda, todos los bordes tienen el mismo estilo de borde. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | establece el formato personalizado, null o cadena vacía significa sin formato personalizado. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Establece una fórmula del [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Establece la fórmula y el valor de la fórmula. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Establece la cadena HTML que contiene datos y algunos formatos en esta celda. |
| [setNumberType(int numbertype)](#setNumberType-int-) | establece el formato de visualización de números y fechas |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Obtiene una copia del estilo de la celda. establece el estilo para la celda. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Obtiene el valor contenido en esta celda. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Cell actual. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Copia datos de una celda origen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Objeto fuente [GridCell](../../com.aspose.gridweb/gridcell). |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


copia el estilo y establece el estilo para la celda

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El estilo de origen. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Crea un objeto de comentario para una celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nota | java.lang.String | nota de comentario. |
| autor | java.lang.String | autor del comentario. |
| isvisible | boolean | si el comentario es visible. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Crea un objeto de validación para una celda.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Tipo de validación. |
| isRequried | boolean | Si el valor de la celda es obligatorio. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Comprueba si este objeto se refiere a la misma celda que otro objeto de celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | otro objeto GridCell |

**Returns:**
booleano - verdadero si dos objetos de celda hacen referencia a la misma celda.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Obtiene el valor booleano contenido en la celda.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtiene el número de columna (basado en cero) de la celda.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Obtener el objeto de comentario en esta celda

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Obtiene el valor DateTime contenido en la celda.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Obtiene el valor de cadena formateado de esta celda.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Obtiene el valor double contenido en la celda.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Obtiene el valor float contenido en la celda.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtiene una fórmula del [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor use siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

El usuario puede establecer cualquier fórmula en el archivo de diseño del Workbook. Aspose.Cells mantendrá todas las fórmulas. Si el usuario usa esta propiedad para establecer una fórmula en una celda, se admite la mayor parte de las funciones integradas del Workbook. Y hay más por venir. Si tiene alguna necesidad especial para las funciones integradas del Workbook, por favor háganoslo saber.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Obtiene la cadena HTML que contiene datos y algunos formatos en esta celda.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Obtiene el valor entero contenido en la celda.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la celda. Por ejemplo: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Obtiene el número de fila (basado en cero) de la celda.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtiene el valor de cadena contenido en la celda.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Obtiene una copia del estilo de la celda. establece el estilo para la celda.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


devuelve el tipo de valor de la celda, el significado se puede ver en GridCellValueType.java

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor contenido en esta celda.

**Remarks**

Tipo posible:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Obtiene el ancho del valor en unidades de píxeles.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Sirve como una función hash para un tipo particular.

**Returns:**
int - Un código hash para el objeto GridCell actual.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Comprueba si una fórmula puede evaluar correctamente un resultado.

**Remarks**

Solo se aplica a la celda de fórmula.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Representa si la celda especificada contiene una fórmula.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado.

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


Inserta un valor booleano en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| param_boolean | boolean | Valor de entrada |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Inserta un valor DateTime en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Valor de entrada |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Inserta un valor double en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| param_double | double | Valor de entrada |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Inserta un valor entero en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| param_int | int | Valor de entrada |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Inserta un valor de objeto en la celda. lo mismo que setValue(Object param\_object)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objectValue | java.lang.Object | valor de entrada |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Inserta un valor de cadena en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| param_string | java.lang.String | Valor de entrada |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Inserta un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |
| isConverted | boolean | True: convertido a otro tipo de datos si es apropiado. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Inserta un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |
| isConverted | boolean | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | boolean | True: establece el formato numérico en el estilo de la celda al convertir a otro tipo de datos |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Establece el valor de la celda con un valor de cadena y establece el formato de la celda según este valor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Elimina el objeto de comentario de la celda.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Elimina el objeto de validación de la celda.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Establece bordes (superior, inferior, izquierdo y derecho) para una celda, todos los bordes tienen el mismo estilo de borde.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | El estilo del borde. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


establece el formato personalizado, null o cadena vacía significa sin formato personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| personalizado | java.lang.String | la presentación de cadena personalizada |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Establece una fórmula del [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor use siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

El usuario puede establecer cualquier fórmula en el archivo de diseño del Workbook. Aspose.Cells mantendrá todas las fórmulas. Si el usuario usa esta propiedad para establecer una fórmula en una celda, se admite la mayor parte de las funciones integradas del Workbook. Y hay más por venir. Si tiene alguna necesidad especial para las funciones integradas del Workbook, por favor háganoslo saber.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Establece la fórmula y el valor de la fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula. |
| valor | java.lang.Object | El valor de la fórmula. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Establece la cadena HTML que contiene datos y algunos formatos en esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


establece el formato de visualización de números y fechas

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| numbertype | int | el valor del numbertype, vea GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Obtiene una copia del estilo de la celda. establece el estilo para la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Obtiene el valor contenido en esta celda.

**Remarks**

Tipo posible:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Cell actual.

**Returns:**
java.lang.String -
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

