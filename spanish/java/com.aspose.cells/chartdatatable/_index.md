---
title: "ChartDataTable"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una tabla de datos del gráfico."
type: docs
url: /es/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Representa una tabla de datos del gráfico.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtiene el modo de visualización del fondo |
| [getBorder()](#getBorder--) | Devuelve un objeto Border que representa el borde del objeto. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) que representa la configuración de fuente de la tabla de datos del gráfico especificada. |
| [getShowLegendKey()](#getShowLegendKey--) | True si la clave de leyenda de la etiqueta de datos es visible. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | True si la tabla de datos del gráfico tiene bordes de celda horizontales |
| [hasBorderOutline()](#hasBorderOutline--) | True si la tabla de datos del gráfico tiene bordes de contorno |
| [hasBorderVertical()](#hasBorderVertical--) | True si la tabla de datos del gráfico tiene bordes de celda verticales |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | True si la tabla de datos del gráfico tiene bordes de celda horizontales |
| [hasOutlineBorder()](#hasOutlineBorder--) | True si la tabla de datos del gráfico tiene bordes de contorno |
| [hasVerticalBorder()](#hasVerticalBorder--) | True si la tabla de datos del gráfico tiene bordes de celda verticales |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Establece el modo de visualización del fondo |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | True si la tabla de datos del gráfico tiene bordes de celda horizontales |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | True si la tabla de datos del gráfico tiene bordes de contorno |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | True si la tabla de datos del gráfico tiene bordes de celda verticales |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | True si la tabla de datos del gráfico tiene bordes de celda horizontales |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | True si la tabla de datos del gráfico tiene bordes de contorno |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | True si la tabla de datos del gráfico tiene bordes de celda verticales |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | True si la clave de leyenda de la etiqueta de datos es visible. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Obtiene el modo de visualización del fondo

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Devuelve un objeto Border que representa el borde del objeto.

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Obtiene un objeto [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) que representa la configuración de fuente de la tabla de datos del gráfico especificada.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


True si la clave de leyenda de la etiqueta de datos es visible.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


True si la tabla de datos del gráfico tiene bordes de celda horizontales

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasHorizontalBorder. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


True si la tabla de datos del gráfico tiene bordes de contorno

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasOutlineBorder. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


True si la tabla de datos del gráfico tiene bordes de celda verticales

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasVerticalBorder. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


True si la tabla de datos del gráfico tiene bordes de celda horizontales

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


True si la tabla de datos del gráfico tiene bordes de contorno

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


True si la tabla de datos del gráfico tiene bordes de celda verticales

**Returns:**
boolean
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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Establece el modo de visualización del fondo

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


True si la tabla de datos del gráfico tiene bordes de celda horizontales

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasHorizontalBorder. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


True si la tabla de datos del gráfico tiene bordes de contorno

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasOutlineBorder. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


True si la tabla de datos del gráfico tiene bordes de celda verticales

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasVerticalBorder. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


True si la tabla de datos del gráfico tiene bordes de celda horizontales

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


True si la tabla de datos del gráfico tiene bordes de contorno

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


True si la tabla de datos del gráfico tiene bordes de celda verticales

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


True si la clave de leyenda de la etiqueta de datos es visible.

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

