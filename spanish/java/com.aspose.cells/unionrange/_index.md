---
title: "UnionRange"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un rango de unión."
type: docs
url: /es/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Representa un rango de unión.
## Métodos

| Método | Descripción |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a todo un rango. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Copiando el rango con opciones de pegado especial. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Obtiene el recuento total de celdas en el rango. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Obtiene la cantidad de filas en el rango. |
| [getFirstColumn()](#getFirstColumn--) | Obtiene el índice de la primera columna del rango. |
| [getFirstRow()](#getFirstRow--) | Obtiene el índice de la primera fila del rango. |
| [getHyperlinks()](#getHyperlinks--) | Obtiene todos los hipervínculos en el rango. |
| [getName()](#getName--) | Obtiene el nombre del rango. |
| [getRangeCount()](#getRangeCount--) | Obtiene el recuento de los rangos. |
| [getRanges()](#getRanges--) | Obtiene todos los rangos de unión. |
| [getRefersTo()](#getRefersTo--) | Obtiene a qué se refiere el rango. |
| [getRowCount()](#getRowCount--) | Obtiene la cantidad de filas en el rango. |
| [getValue()](#getValue--) | Obtiene los valores del rango. |
| [hasRange()](#hasRange--) | Indica si esto tiene rango. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Interseca otro rango. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Interseca otro rango. |
| [intersect(String range)](#intersect-java.lang.String-) | Interseca otro rango. |
| [iterator()](#iterator--) | Obtiene el enumerador de celdas en este Range. |
| [merge()](#merge--) | Combina un rango de celdas en una sola celda. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Introduce un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre del rango. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Establece los bordes de contorno alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Establece los bordes externos alrededor de un rango de celdas. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Establece el estilo del rango. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece los valores del rango. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Descombina celdas combinadas de este rango. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Une los rangos. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Une otro rango. |
| [union(String range)](#union-java.lang.String-) | Une otro rango. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Aplica formatos a todo un rango.

**Remarks**

Cada celda en este rango contendrá un objeto [Style](../../com.aspose.cells/style). Por lo tanto, este es un método que consume mucha memoria. Por favor, úselo con cuidado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Copiando el rango con opciones de pegado especial.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | El rango de origen. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Las opciones de pegado especial. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Obtiene el recuento total de celdas en el rango.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Obtiene la cantidad de filas en el rango.

**Remarks**

Solo tiene efecto cuando solo contiene un rango.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Obtiene el índice de la primera columna del rango.

**Remarks**

Solo tiene efecto cuando solo contiene un rango.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Obtiene el índice de la primera fila del rango.

**Remarks**

Solo tiene efecto cuando solo contiene un rango.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Obtiene todos los hipervínculos en el rango.

**Returns:**
com.aspose.cells.Hyperlink[]
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del rango.

**Remarks**

Se admite rango con nombre. Por ejemplo,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Obtiene el recuento de los rangos.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Obtiene todos los rangos de unión.

**Returns:**
com.aspose.cells.Range[]
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Obtiene a qué se refiere el rango.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtiene la cantidad de filas en el rango.

**Remarks**

Solo tiene efecto cuando solo contiene un rango.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene los valores del rango.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Indica si esto tiene rango.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Interseca otro rango.

**Remarks**

Si los dos rangos de unión no se intersectan, devuelve nulo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | El rango. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Interseca otro rango.

**Remarks**

Si los dos rangos de unión no se intersectan, devuelve nulo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | El rango. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Interseca otro rango.

**Remarks**

Si los dos rangos de unión no se intersectan, devuelve nulo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | java.lang.String | El rango. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de celdas en este Range.

**Remarks**

Al recorrer los elementos mediante el Enumerator devuelto, la colección de celdas no debe modificarse (por ejemplo, operaciones que provoquen la creación de una nueva Cell/Row o la eliminación de una Cell/Row existente). De lo contrario, el enumerador podría no ser capaz de recorrer todas las celdas correctamente (algunos elementos podrían recorrerse repetidamente o omitirse).

**Returns:**
java.util.Iterator - El enumerador de celdas
### merge() {#merge--}
```
public void merge()
```


Combina un rango de celdas en una sola celda.

**Remarks**

Referencia la celda combinada mediante la dirección de la celda superior izquierda del rango.

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Introduce un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |
| isConverted | boolean | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | boolean | True: establece el formato numérico en el estilo de la celda al convertir a otro tipo de datos |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre del rango.

**Remarks**

Se admite rango con nombre. Por ejemplo,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Establece los bordes de contorno alrededor de un rango de celdas con el mismo estilo y color de borde.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilo de borde. |
| borderColor | [Color](../../com.aspose.cells/color) | Color del borde. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Establece los bordes externos alrededor de un rango de celdas.

**Remarks**

Ambas longitudes de borderStyles y borderStyles deben ser 4. El orden de borderStyles y borderStyles debe ser top,bottom,left,right

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilos de borde. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Colores del borde. |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Establece el estilo del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto Style. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Establece los valores del rango.

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
### unMerge() {#unMerge--}
```
public void unMerge()
```


Descombina celdas combinadas de este rango.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Une los rangos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Los rangos. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Une otro rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | El rango. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Une otro rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | java.lang.String | El rango. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

