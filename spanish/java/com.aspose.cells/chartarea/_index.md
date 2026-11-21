---
title: "ChartArea"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa el área del gráfico en la hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/chartarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class ChartArea extends ChartFrame
```

Encapsula el objeto que representa el área del gráfico en la hoja de cálculo.

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
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Getting Chart Area
         ChartArea chartArea = chart.getChartArea();
 
         //Setting the foreground color of the chart area
         chartArea.getArea().setForegroundColor(Color.getYellow());
 
         //Setting Chart Area Shadow
         chartArea.setShadow(true);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtiene el [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [getBackground()](#getBackground--) | Obtiene el modo de visualización del fondo. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtiene el modo de visualización del fondo. |
| [getBorder()](#getBorder--) | Obtiene el [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Obtiene el gráfico al que pertenece este objeto. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Representa la altura de la posición predeterminada en unidades de 1/4000 del área del gráfico. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Representa la altura de la posición predeterminada en unidades de la fracción del área del gráfico. |
| [getDefaultWidth()](#getDefaultWidth--) | Representa el ancho de la posición predeterminada en unidades de 1/4000 del área del gráfico. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Representa el ancho de la posición predeterminada en unidades de fracción del área del gráfico. |
| [getDefaultX()](#getDefaultX--) | Representa la x de la posición predeterminada en unidades de 1/4000 del área del gráfico. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Representa la x de la posición predeterminada en unidades de fracción del área del gráfico. |
| [getDefaultY()](#getDefaultY--) | Representa la y de la posición predeterminada en unidades de 1/4000 del área del gráfico. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Representa la y de la posición predeterminada en unidades de la fracción del área del gráfico. |
| [getFont()](#getFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/chartarea\#getFont--) del objeto ChartArea especificado. |
| [getHeight()](#getHeight--) | Obtiene el desplazamiento vertical desde su fila de esquina inferior\\u9225\\u6186ight, en unidades de 1/4000 del área del gráfico. |
| [getHeightPixel()](#getHeightPixel--) | Obtiene la altura del marco en unidades de píxeles. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Obtiene el desplazamiento vertical desde su fila de esquina inferior derecha, en unidades de proporción del área del gráfico. |
| [getShadow()](#getShadow--) | Verdadero si el marco tiene una sombra. |
| [getShapeProperties()](#getShapeProperties--) | Obtiene el objeto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getTextFont()](#getTextFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado. |
| [getTextOptions()](#getTextOptions--) | Obtiene las opciones del texto. |
| [getWidth()](#getWidth--) | Obtiene el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de 1/4000 del área del gráfico. |
| [getWidthPixel()](#getWidthPixel--) | Obtiene el ancho del marco en unidades de píxel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Obtiene el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de proporción del área del gráfico. |
| [getX()](#getX--) | Obtiene el desplazamiento horizontal desde su columna de esquina superior izquierda, en unidades de 1/4000 del área del gráfico. |
| [getXPixel()](#getXPixel--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de píxel. |
| [getXRatioToChart()](#getXRatioToChart--) | Obtiene el desplazamiento horizontal desde la columna de esquina superior izquierda, como una proporción del área del gráfico. |
| [getY()](#getY--) | Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de 1/4000 del área del gráfico. |
| [getYPixel()](#getYPixel--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles. |
| [getYRatioToChart()](#getYRatioToChart--) | Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de proporción del área del gráfico. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Indica si el marco del gráfico tiene tamaño automático. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida. |
| [isInnerMode()](#isInnerMode--) | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indica si el marco del gráfico tiene tamaño automático. |
| [setBackground(int value)](#setBackground-int-) | Establece el modo de visualización del fondo. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Establece el modo de visualización del fondo. |
| [setHeight(int value)](#setHeight-int-) | Establece el desplazamiento vertical desde su fila de esquina inferior\\u9225\\u6186ight, en unidades de 1/4000 del área del gráfico. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Establece la altura del marco en unidades de píxeles. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Establece el desplazamiento vertical desde su fila de esquina inferior derecha, en unidades de proporción del área del gráfico. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. |
| [setPositionAuto()](#setPositionAuto--) | Establece la posición del marco a automática |
| [setShadow(boolean value)](#setShadow-boolean-) | Verdadero si el marco tiene una sombra. |
| [setWidth(int value)](#setWidth-int-) | Establece el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de 1/4000 del área del gráfico. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Establece el ancho del marco en unidades de píxel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Establece el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de proporción del área del gráfico. |
| [setX(int value)](#setX-int-) | Establece el desplazamiento horizontal desde su columna de esquina superior izquierda, en unidades de 1/4000 del área del gráfico. |
| [setXPixel(int value)](#setXPixel-int-) | Establece la coordenada x de la esquina superior izquierda en unidades de píxel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Establece el desplazamiento horizontal desde la columna de esquina superior izquierda, como una proporción del área del gráfico. |
| [setY(int value)](#setY-int-) | Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de 1/4000 del área del gráfico. |
| [setYPixel(int value)](#setYPixel-int-) | Establece la coordenada y de la esquina superior izquierda en unidades de píxeles. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de proporción del área del gráfico. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Obtiene el [getArea()](../../com.aspose.cells/chartframe\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Obtiene el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de ENERO de 2012. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Obtiene el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de febrero de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Obtiene el [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Obtiene el gráfico al que pertenece este objeto.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Representa la altura de la posición predeterminada en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.DefaultHeightRatioToChart, en su lugar. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Representa la altura de la posición predeterminada en unidades de la fracción del área del gráfico.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Representa el ancho de la posición predeterminada en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.DefaultWidthRatioToChart, en su lugar. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Representa el ancho de la posición predeterminada en unidades de fracción del área del gráfico.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Representa la x de la posición predeterminada en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.DefaultXRatioToChart, en su lugar. DefaultX = (int)(DefaultXRatioToChart \* 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Representa la x de la posición predeterminada en unidades de fracción del área del gráfico.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Representa la y de la posición predeterminada en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.DefaultYRatioToChart, en su lugar. DefaultY = (int)(DefaultYRatioToChart \* 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Representa la y de la posición predeterminada en unidades de la fracción del área del gráfico.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Obtiene un objeto [getFont()](../../com.aspose.cells/chartarea\#getFont--) del objeto ChartArea especificado.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Obtiene el desplazamiento vertical desde su fila de esquina inferior\\u9225\\u6186ight, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.HeightRatioToChart, en su lugar. Height = HeightRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Obtiene la altura del marco en unidades de píxeles.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Obtiene el desplazamiento vertical desde su fila de esquina inferior derecha, en unidades de proporción del área del gráfico.

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Verdadero si el marco tiene una sombra.

**Remarks**

Solo para gráficos en archivo xls.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtiene el objeto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--).

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Font. Esta propiedad será eliminada 12 meses después desde enero de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Obtiene las opciones del texto.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Obtiene el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.WidthRatioToChart, en su lugar. Width = WidthRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Obtiene el ancho del marco en unidades de píxel.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Obtiene el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de proporción del área del gráfico.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Obtiene el desplazamiento horizontal desde su columna de esquina superior izquierda, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.XRatioToChart, en su lugar. X = XRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Obtiene la coordenada x de la esquina superior izquierda en unidades de píxel.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Obtiene el desplazamiento horizontal desde la columna de esquina superior izquierda, como una proporción del área del gráfico.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.YRatioToChart, en su lugar. Y = YRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de proporción del área del gráfico.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Indica si el marco del gráfico tiene tamaño automático.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de graduación y las etiquetas de los ejes.

**Remarks**

Solo para archivo Xlsx.

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Indica si el marco del gráfico tiene tamaño automático.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de ENERO de 2012. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de febrero de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Establece el desplazamiento vertical desde su fila de esquina inferior\\u9225\\u6186ight, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.HeightRatioToChart, en su lugar. Height = HeightRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Establece la altura del marco en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Establece el desplazamiento vertical desde su fila de esquina inferior derecha, en unidades de proporción del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de graduación y las etiquetas de los ejes.

**Remarks**

Solo para archivo Xlsx.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Establece la posición del marco a automática

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Verdadero si el marco tiene una sombra.

**Remarks**

Solo para gráficos en archivo xls.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Establece el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.WidthRatioToChart, en su lugar. Width = WidthRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Establece el ancho del marco en unidades de píxel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Establece el desplazamiento horizontal desde su columna de esquina inferior derecha, en unidades de proporción del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Establece el desplazamiento horizontal desde su columna de esquina superior izquierda, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.XRatioToChart, en su lugar. X = XRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Establece la coordenada x de la esquina superior izquierda en unidades de píxel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Establece el desplazamiento horizontal desde la columna de esquina superior izquierda, como una proporción del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.YRatioToChart, en su lugar. Y = YRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Establece la coordenada y de la esquina superior izquierda en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Obtiene o obtiene el desplazamiento vertical desde su fila de esquina superior izquierda, en unidades de proporción del área del gráfico.

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

