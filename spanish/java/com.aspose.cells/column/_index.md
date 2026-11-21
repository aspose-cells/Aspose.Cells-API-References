---
title: "Column"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una sola columna en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Representa una sola columna en una hoja de cálculo.

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
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a una columna completa. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Obtiene el nivel de grupo de la columna. |
| [getIndex()](#getIndex--) | Obtiene el índice de esta columna. |
| [getStyle()](#getStyle--) | Obtiene el estilo de esta columna. |
| [getWidth()](#getWidth--) | Obtiene el ancho de la columna en unidades de caracteres. |
| [hasCustomStyle()](#hasCustomStyle--) | Indica si esta columna tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro de trabajo). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | si la columna está colapsada |
| [isHidden()](#isHidden--) | Indica si la columna está oculta. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | si la columna está colapsada |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Obtiene el nivel de grupo de la columna. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica si la columna está oculta. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Establece el estilo de esta columna. |
| [setWidth(double value)](#setWidth-double-) | Establece el ancho de la columna en unidades de caracteres. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Aplica formatos a una columna completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Obtiene el nivel de grupo de la columna.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de esta columna.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtiene el estilo de esta columna.

**Remarks**

Modificar directamente el objeto de estilo devuelto no tiene efecto en esta columna ni en ninguna celda de esta columna. Debes llamar al método [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) o [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) para aplicar el cambio a esta columna.

El estilo de la columna es el estilo que será heredado por las celdas de esta columna (aquellas celdas que no tienen configuraciones de estilo personalizadas, como celdas existentes que no se les ha asignado estilo explícitamente, o aquellas que no han sido instanciadas)

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtiene el ancho de la columna en unidades de caracteres.

**Remarks**

Para la hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígitos de los números 0~9 tal como se renderizan en la fuente del estilo normal.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indica si esta columna tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro de trabajo).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


si la columna está colapsada

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica si la columna está oculta.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


si la columna está colapsada

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Obtiene el nivel de grupo de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica si la columna está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Establece el estilo de esta columna.

**Remarks**

Este método solo establece el estilo dado como el estilo predeterminado para esta columna, sin cambiar la configuración de estilo de las celdas existentes en esta columna. Para actualizar la configuración de estilo de las celdas existentes al estilo especificado al mismo tiempo, por favor use [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | el estilo que se usará como estilo predeterminado para las celdas en esta columna. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Establece el ancho de la columna en unidades de caracteres.

**Remarks**

Para la hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígitos de los números 0~9 tal como se renderizan en la fuente del estilo normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

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

