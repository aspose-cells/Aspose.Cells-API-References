---
title: "FindOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de búsqueda."
type: docs
url: /es/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Representa las opciones de búsqueda.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Indica si la cadena buscada distingue entre mayúsculas y minúsculas. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Obtiene un valor que indica si se convierte el valor de cadena buscada a datos numéricos. |
| [getLookAtType()](#getLookAtType--) | Tipo de búsqueda 'look at'. |
| [getLookInType()](#getLookInType--) | Tipo de búsqueda 'look in'. |
| [getRange()](#getRange--) | Obtiene y establece el rango buscado. |
| [getRegexKey()](#getRegexKey--) | Indica si la clave buscada es una expresión regular. |
| [getSearchBackward()](#getSearchBackward--) | Si buscar hacia atrás en celdas. |
| [getSearchNext()](#getSearchNext--) | Orden de búsqueda. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Indica si el orden de búsqueda es por filas o columnas. |
| [getStyle()](#getStyle--) | El formato a buscar. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Indica si el rango buscado está establecido. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Indica si la cadena buscada distingue entre mayúsculas y minúsculas. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Establece un valor que indica si se convierte el valor de cadena buscado a datos numéricos. |
| [setLookAtType(int value)](#setLookAtType-int-) | Tipo de búsqueda 'look at'. |
| [setLookInType(int value)](#setLookInType-int-) | Tipo de búsqueda 'look in'. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Establece el rango buscado. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Indica si la clave buscada es una expresión regular. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Si buscar hacia atrás en celdas. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Orden de búsqueda. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Indica si el orden de búsqueda es por filas o columnas. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | El formato a buscar. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
```


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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Indica si la cadena buscada distingue entre mayúsculas y minúsculas.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtiene un valor que indica si se convierte el valor de cadena buscada a datos numéricos.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Tipo de búsqueda 'look at'.

Ver [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Cuando [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) es verdadero y el usuario ha especificado la regla exacta para la expresión regular, por consideraciones de rendimiento esta propiedad debe establecerse como [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). De lo contrario, reformaremos la clave de búsqueda para garantizar que pueda coincidir según el tipo específico. Por ejemplo, cuando el tipo es [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (este es el valor predeterminado para esta propiedad), añadiremos comodines al inicio y al final de la clave de búsqueda automáticamente. En este caso, las expresiones regulares se volverán más complejas y el rendimiento también disminuirá.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Tipo de búsqueda 'look in'.

Ver [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Obtiene y establece el rango buscado.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Indica si la clave buscada es una expresión regular. Si es verdadero, la clave buscada se tomará como expresión regular y se analizará. De lo contrario, la clave se analizará según las reglas de MS Excel.

**Remarks**

Aunque la clave de búsqueda se haya especificado como expresión regular, puede ser reformada según el [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) especificado. Por ejemplo, cuando el tipo es [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (este es el valor predeterminado para estas opciones), se añadirán comodines al inicio y al final de la clave de búsqueda automáticamente para asegurar que la coincidencia se verifique como "contiene". En este caso, las expresiones regulares se volverán más complejas y el rendimiento también disminuirá. Por lo tanto, por consideraciones de rendimiento, si el usuario ha especificado la regla exacta para la expresión regular, no es necesario usar [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) como restricción adicional y el usuario puede establecerlo como [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) para obtener mejor rendimiento.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Si buscar hacia atrás en celdas.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Orden de búsqueda. Verdadero: buscar siguiente. Falso: buscar anterior.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad FindOptions.SearchBackward. Esta propiedad será eliminada 12 meses después desde noviembre de 2018. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Indica si el orden de búsqueda es por filas o columnas.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


El formato a buscar.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Indica si el rango buscado está establecido.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Indica si la cadena buscada distingue entre mayúsculas y minúsculas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Establece un valor que indica si se convierte el valor de cadena buscado a datos numéricos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Tipo de búsqueda 'look at'.

Ver [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Cuando [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) es verdadero y el usuario ha especificado la regla exacta para la expresión regular, por consideraciones de rendimiento esta propiedad debe establecerse como [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). De lo contrario, reformaremos la clave de búsqueda para garantizar que pueda coincidir según el tipo específico. Por ejemplo, cuando el tipo es [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (este es el valor predeterminado para esta propiedad), añadiremos comodines al inicio y al final de la clave de búsqueda automáticamente. En este caso, las expresiones regulares se volverán más complejas y el rendimiento también disminuirá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


Tipo de búsqueda 'look in'.

Ver [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Establece el rango buscado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | el rango buscado. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Indica si la clave buscada es una expresión regular. Si es verdadero, la clave buscada se tomará como expresión regular y se analizará. De lo contrario, la clave se analizará según las reglas de MS Excel.

**Remarks**

Aunque la clave de búsqueda se haya especificado como expresión regular, puede ser reformada según el [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) especificado. Por ejemplo, cuando el tipo es [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (este es el valor predeterminado para estas opciones), se añadirán comodines al inicio y al final de la clave de búsqueda automáticamente para asegurar que la coincidencia se verifique como "contiene". En este caso, las expresiones regulares se volverán más complejas y el rendimiento también disminuirá. Por lo tanto, por consideraciones de rendimiento, si el usuario ha especificado la regla exacta para la expresión regular, no es necesario usar [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) como restricción adicional y el usuario puede establecerlo como [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) para obtener mejor rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Si buscar hacia atrás en celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Orden de búsqueda. Verdadero: buscar siguiente. Falso: buscar anterior.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad FindOptions.SearchBackward. Esta propiedad será eliminada 12 meses después desde noviembre de 2018. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Indica si el orden de búsqueda es por filas o columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


El formato a buscar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Indica si el tipo de valor de la celda buscada debe ser el mismo que la clave buscada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

