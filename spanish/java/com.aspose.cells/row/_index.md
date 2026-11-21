---
title: "Row"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una fila única en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Representa una fila única en una hoja de cálculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a una fila completa. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Copia la configuración de la fila, como estilo, altura, visibilidad, ...etc. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Comprueba si este objeto se refiere a la misma fila que otro objeto fila. |
| [equals(Object obj)](#equals-java.lang.Object-) | Comprueba si este objeto se refiere a la misma fila que otro. |
| [get(int column)](#get-int-) | Obtiene la celda. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Obtiene la celda por un índice específico en la colección de celdas de esta fila. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Obtiene la celda o null en el índice específico. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Obtiene el primer objeto celda en la fila. |
| [getFirstDataCell()](#getFirstDataCell--) | Obtiene la primera celda no vacía en la fila. |
| [getGroupLevel()](#getGroupLevel--) | Obtiene el nivel de grupo de la fila. |
| [getHeight()](#getHeight--) | Obtiene la altura de la fila en unidades de puntos. |
| [getIndex()](#getIndex--) | Obtiene el índice de esta fila. |
| [getLastCell()](#getLastCell--) | Obtiene el último objeto celda en la fila. |
| [getLastDataCell()](#getLastDataCell--) | Obtiene la última celda no vacía en la fila. |
| [getStyle()](#getStyle--) | Obtiene el estilo de esta fila. |
| [hasCustomStyle()](#hasCustomStyle--) | Indica si esta fila tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro de trabajo). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indica si la fila contiene algún dato |
| [isCollapsed()](#isCollapsed--) | si la fila está colapsada |
| [isHeightMatched()](#isHeightMatched--) | Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. |
| [isHidden()](#isHidden--) | Indica si la fila está oculta. |
| [iterator()](#iterator--) | Obtiene el enumerador de celdas |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Obtiene un enumerador que recorre las celdas de esta fila. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | si la fila está colapsada |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Obtiene el nivel de grupo de la fila. |
| [setHeight(double value)](#setHeight-double-) | Establece la altura de la fila en unidades de puntos. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica si la fila está oculta. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Establece el estilo de esta fila. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Aplica formatos a una fila completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Copia la configuración de la fila, como estilo, altura, visibilidad, ...etc.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | la fila origen cuyas configuraciones se copiarán a esta |
| checkStyle | boolean | si se verifica y recopila el estilo. Solo tiene efecto y es necesario cuando dos objetos fila pertenecen a diferentes libros y los estilos de los dos libros son diferentes. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Comprueba si este objeto se refiere a la misma fila que otro objeto fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | otro objeto fila |

**Returns:**
booleano - verdadero si dos objetos fila se refieren a la misma fila.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Comprueba si este objeto se refiere a la misma fila que otro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | otro objeto |

**Returns:**
booleano - verdadero si dos objetos se refieren a la misma fila.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Obtiene la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Obtiene la celda por un índice específico en la colección de celdas de esta fila.

**Remarks**

Para recorrer todas las celdas en secuencia sin modificar, usar [iterator()](../../com.aspose.cells/row\#iterator--) ofrecerá mejor rendimiento que usar este método para obtener celdas una por una.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice (posición) de la celda en la colección de celdas de esta fila. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Obtiene la celda o null en el índice específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Obtiene el primer objeto celda en la fila.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Obtiene la primera celda no vacía en la fila.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Obtiene el nivel de grupo de la fila.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtiene la altura de la fila en unidades de puntos.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de esta fila.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Obtiene el último objeto celda en la fila.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Obtiene la última celda no vacía en la fila.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtiene el estilo de esta fila.

**Remarks**

Modificar directamente el objeto de estilo devuelto no tiene efecto en esta fila ni en ninguna celda de ella. Debe llamar al método [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) o [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) para aplicar el cambio a esta fila.

El estilo de la fila es el estilo que heredarán las celdas de esta fila (aquellas celdas que no tienen configuraciones de estilo personalizadas, como celdas existentes que no se les ha asignado estilo explícitamente, o aquellas que no se han instanciado).

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indica si esta fila tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro de trabajo).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indica si la fila contiene algún dato

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


si la fila está colapsada

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. Verdadero en esta propiedad también indica que la altura de la fila es \"automática\" sin un valor de altura personalizado establecido por el usuario.

**Remarks**

Cuando esta propiedad es verdadera, si el contenido de esta fila cambia, generalmente la altura de la fila necesita recalcularse (por ejemplo mediante [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) para obtener el mismo resultado que se muestra en MS Excel al abrir el libro.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica si la fila está oculta.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de celdas

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - El enumerador de celdas que recorrerá todas las celdas existentes en esta fila.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Obtiene un enumerador que recorre las celdas de esta fila.

**Remarks**

Si la fila se va a modificar (por operaciones que pueden causar la instanciación de una nueva Celda o la eliminación de una Celda existente) durante el recorrido con el enumerador, se debe usar un enumerador sincronizado en lugar del enumerador normal para que el recorrido pueda continuar desde la posición justo después de la que fue recorrida por el último MoveNext(). Sin embargo, junto con la ventaja de que no se omita ni recorra repetidamente ningún elemento, la desventaja del enumerador sincronizado es que el rendimiento se degradará un poco en comparación con el enumerador normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| revertido | boolean | si enumerar celdas en orden inverso |
| sincronizar | boolean | si el enumerador devuelto debe comprobar la modificación de celdas en esta fila y mantenerse sincronizado con ella. |

**Returns:**
java.util.Iterator - El enumerador de celdas que recorrerá todas las celdas existentes en esta fila.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


si la fila está colapsada

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Obtiene el nivel de grupo de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Establece la altura de la fila en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. Verdadero en esta propiedad también indica que la altura de la fila es \"automática\" sin un valor de altura personalizado establecido por el usuario.

**Remarks**

Cuando esta propiedad es verdadera, si el contenido de esta fila cambia, generalmente la altura de la fila necesita recalcularse (por ejemplo mediante [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) para obtener el mismo resultado que se muestra en MS Excel al abrir el libro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica si la fila está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Establece el estilo de esta fila.

**Remarks**

Este método solo establece el estilo dado como el estilo predeterminado para esta fila, sin cambiar la configuración de estilo de las celdas existentes en esta fila. Para actualizar la configuración de estilo de las celdas existentes al estilo especificado al mismo tiempo, por favor use [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | el estilo que se usará como estilo predeterminado para las celdas en esta fila. |

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

