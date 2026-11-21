---
title: "DataLabels"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de todos los objetos DataLabel para la Serie especificada."
type: docs
url: /es/java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

Encapsula una colección de todos los objetos DataLabel para la Serie especificada.

**Example**

```
         //Set the DataLabels in the chart
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         DataLabels datalabels;
         for (int i = 0; i  <chart.getNSeries().getCount(); i++)
         {
             datalabels = chart.getNSeries().get(i).getDataLabels();
             //Set the position of DataLabels
             datalabels.setPosition(LabelPositionType.INSIDE_BASE);
             //Show the category name in the DataLabels
             datalabels.setShowCategoryName(true);
             //Show the value in the DataLabels
             datalabels.setShowValue(true);
             //Not show the percentage in the DataLabels
             datalabels.setShowPercentage(false);
             //Not show the legend key.
             datalabels.setShowLegendKey(false);
         }
```
## Métodos

| Método | Descripción |
| --- | --- |
| [applyFont()](#applyFont--) | Aplicar la fuente de las etiquetas de datos a todos los nodos hijos. |
| [characters(int startIndex, int length)](#characters-int-int-) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtiene el [getArea()](../../com.aspose.cells/datalabels\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [getBackground()](#getBackground--) | Obtiene el modo de visualización del fondo. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtiene el modo de visualización del fondo |
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
| [getDirectionType()](#getDirectionType--) | Obtiene la dirección del texto. |
| [getFont()](#getFont--) | Obtiene la fuente de las DataLabels; |
| [getHeight()](#getHeight--) | Obtiene la altura del marco en unidades de 1/4000 del área del gráfico. |
| [getHeightPixel()](#getHeightPixel--) | Obtiene la altura del marco en unidades de píxeles. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Obtiene la altura del marco en unidades de la proporción del área del gráfico. |
| [getLinkedSource()](#getLinkedSource--) | Obtiene una referencia a la hoja de cálculo. |
| [getNumber()](#getNumber--) | Obtiene el formato numérico incorporado. |
| [getNumberFormat()](#getNumberFormat--) | Representa la cadena de formato para el objeto DataLabels. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas). |
| [getPosition()](#getPosition--) | Representa la posición de la etiqueta de datos. |
| [getReadingOrder()](#getReadingOrder--) | Representa el orden de lectura del texto. |
| [getRotationAngle()](#getRotationAngle--) | Representa el ángulo de rotación del texto. |
| [getSeparatorType()](#getSeparatorType--) | Obtiene el tipo de separador usado para las etiquetas de datos en un gráfico. |
| [getSeparatorValue()](#getSeparatorValue--) | Obtiene el valor del separador usado para las etiquetas de datos en un gráfico. |
| [getShadow()](#getShadow--) | Verdadero si el marco tiene una sombra. |
| [getShapeProperties()](#getShapeProperties--) | Obtiene el objeto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getShapeType()](#getShapeType--) | Obtiene el tipo de forma de la etiqueta de datos. |
| [getShowBubbleSize()](#getShowBubbleSize--) | Representa el comportamiento de visualización del valor porcentual de la etiqueta de datos de un gráfico especificado. |
| [getShowCategoryName()](#getShowCategoryName--) | Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. Verdadero para mostrar el nombre de categoría de las etiquetas de datos en un gráfico. |
| [getShowCellRange()](#getShowCellRange--) | Indica si se muestra el rango de celdas como etiquetas de datos. |
| [getShowLegendKey()](#getShowLegendKey--) | Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. |
| [getShowPercentage()](#getShowPercentage--) | Representa el comportamiento de visualización del valor porcentual de la etiqueta de datos de un gráfico especificado. |
| [getShowSeriesName()](#getShowSeriesName--) | Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. |
| [getShowValue()](#getShowValue--) | Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. |
| [getText()](#getText--) | Obtiene el texto de la etiqueta de datos. |
| [getTextDirection()](#getTextDirection--) | Representa el orden de lectura del texto. |
| [getTextFont()](#getTextFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtiene la alineación horizontal del texto. |
| [getTextOptions()](#getTextOptions--) | Obtiene las opciones del texto. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtiene la alineación vertical del texto. |
| [getWidth()](#getWidth--) | Obtiene el ancho del marco en unidades de 1/4000 del área del gráfico. |
| [getWidthPixel()](#getWidthPixel--) | Obtiene el ancho del marco en unidades de píxel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Obtiene el ancho del marco en unidades de la proporción del área del gráfico. |
| [getX()](#getX--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [getXPixel()](#getXPixel--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de píxel. |
| [getXRatioToChart()](#getXRatioToChart--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de proporción del área del gráfico. |
| [getY()](#getY--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [getYPixel()](#getYPixel--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles. |
| [getYRatioToChart()](#getYRatioToChart--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de la proporción del área del gráfico. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indica que el texto se genera automáticamente. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indica si el texto del gráfico se rota automáticamente. |
| [isAutomaticSize()](#isAutomaticSize--) | Indica si el marco del gráfico tiene tamaño automático. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida. |
| [isDeleted()](#isDeleted--) | Indica si esta etiqueta de datos está eliminada. |
| [isInnerMode()](#isInnerMode--) | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. |
| [isNeverOverlap()](#isNeverOverlap--) | Indica si las etiquetas de datos nunca se superponen al generar una imagen de gráfico circular. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Obtiene si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. |
| [isTextWrapped()](#isTextWrapped--) | Obtiene un valor que indica si el texto está ajustado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indica que el texto se genera automáticamente. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indica si el marco del gráfico tiene tamaño automático. |
| [setBackground(int value)](#setBackground-int-) | Establece el modo de visualización del fondo. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Establece el modo de visualización del fondo |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indica si esta etiqueta de datos está eliminada. |
| [setDirectionType(int value)](#setDirectionType-int-) | Establece la dirección del texto. |
| [setHeight(int value)](#setHeight-int-) | Establece la altura del marco en unidades de 1/4000 del área del gráfico. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Establece la altura del marco en unidades de píxeles. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Establece la altura del marco en unidades de la proporción del área del gráfico. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Establece una referencia a la hoja de cálculo. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | Indica si las etiquetas de datos nunca se superponen al generar una imagen de gráfico circular. |
| [setNumber(int value)](#setNumber-int-) | Establece el formato numérico incorporado. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Representa la cadena de formato para el objeto DataLabels. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas). |
| [setPosition(int value)](#setPosition-int-) | Representa la posición de la etiqueta de datos. |
| [setPositionAuto()](#setPositionAuto--) | Establece la posición del marco a automática |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Representa el orden de lectura del texto. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representa el ángulo de rotación del texto. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | Establece el tipo de separador usado para las etiquetas de datos en un gráfico. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | Establece el valor del separador usado para las etiquetas de datos en un gráfico. |
| [setShadow(boolean value)](#setShadow-boolean-) | Verdadero si el marco tiene una sombra. |
| [setShapeType(int value)](#setShapeType-int-) | Establece el tipo de forma de la etiqueta de datos. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | Representa el comportamiento de visualización del valor porcentual de la etiqueta de datos de un gráfico especificado. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. Verdadero para mostrar el nombre de categoría de las etiquetas de datos en un gráfico. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | Indica si se muestra el rango de celdas como etiquetas de datos. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | Representa el comportamiento de visualización del valor porcentual de la etiqueta de datos de un gráfico especificado. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto de la etiqueta de datos. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representa el orden de lectura del texto. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Establece la alineación horizontal del texto. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Establece la alineación vertical del texto. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Establece un valor que indica si el texto está ajustado. |
| [setWidth(int value)](#setWidth-int-) | Establece el ancho del marco en unidades de 1/4000 del área del gráfico. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Establece el ancho del marco en unidades de píxel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Establece el ancho del marco en unidades de proporción del área del gráfico. |
| [setX(int value)](#setX-int-) | Establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [setXPixel(int value)](#setXPixel-int-) | Establece la coordenada x de la esquina superior izquierda en unidades de píxel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Establece la coordenada x de la esquina superior izquierda en unidades de proporción del área del gráfico. |
| [setY(int value)](#setY-int-) | Establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [setYPixel(int value)](#setYPixel-int-) | Establece la coordenada y de la esquina superior izquierda en unidades de píxeles. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Establece la coordenada y de la esquina superior izquierda en unidades de la proporción del área del gráfico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


Aplicar la fuente de las etiquetas de datos a todos los nodos hijos.

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Devuelve un objeto Characters que representa un rango de caracteres dentro del texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice del inicio del carácter. |
| length | int | El número de caracteres. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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


Obtiene el [getArea()](../../com.aspose.cells/datalabels\#getArea--).

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


Obtiene el modo de visualización del fondo

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

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
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Obtiene la dirección del texto.

Ver [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Obtiene la fuente de las DataLabels;

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Obtiene la altura del marco en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.HeightRatioToChart, en su lugar. Height = HeightRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

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


Obtiene la altura del marco en unidades de la proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de proporción a píxeles? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Obtiene una referencia a la hoja de cálculo.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Obtiene el formato numérico incorporado.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Representa la cadena de formato para el objeto DataLabels.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


Representa la posición de la etiqueta de datos.

Ver [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representa el ángulo de rotación del texto.

**Remarks**


0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.


**Returns:**
int
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


Obtiene el tipo de separador usado para las etiquetas de datos en un gráfico.

Ver [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Para establecer un separador personalizado, establezca la propiedad [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) como [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) y luego especifique el valor esperado para [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


Obtiene el valor del separador usado para las etiquetas de datos en un gráfico.

**Returns:**
java.lang.String
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
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


Obtiene el tipo de forma de la etiqueta de datos.

Ver [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor del porcentaje. False oculta el valor del porcentaje.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado.True para mostrar el nombre de categoría de las etiquetas de datos en un gráfico. False para ocultar.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


Indica si se muestra el rango de celdas como etiquetas de datos.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. True si la clave de leyenda de la etiqueta de datos es visible.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor del porcentaje. False oculta el valor del porcentaje.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. True para mostrar el nombre de la serie. False para ocultar.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. True muestra los valores. False para ocultar.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto de la etiqueta de datos.

**Remarks**

Solo funciona cuando esto es una etiqueta de datos de un punto de gráfico.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartTextFrame.ReadingOrder. Esta propiedad será eliminada 12 meses después desde marzo de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Font. Esta propiedad será eliminada 12 meses después desde enero de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Obtiene la alineación horizontal del texto.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Obtiene las opciones del texto.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Obtiene la alineación vertical del texto.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Obtiene el ancho del marco en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.WidthRatioToChart, en su lugar. Width = WidthRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Obtiene el ancho del marco en unidades de la proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de razón a píxeles? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.XRatioToChart, en su lugar. X = XRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Obtiene la coordenada x de la esquina superior izquierda en unidades de proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de razón a píxeles? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.YRatioToChart, en su lugar. Y = YRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Obtiene la coordenada y de la esquina superior izquierda en unidades de la proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de razón a píxeles? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


Indica que el texto se genera automáticamente.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indica si el texto del gráfico se rota automáticamente.

**Returns:**
boolean
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
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indica si esta etiqueta de datos está eliminada.

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
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


Indica si las etiquetas de datos nunca se superponen al generar una imagen de un gráfico circular. Nota: esta propiedad solo tiene sentido cuando se trata de un gráfico circular a imagen.

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Obtiene si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. El ajuste automático ocurre cuando el texto dentro de una forma se escala para contener todo el texto.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtiene un valor que indica si el texto está ajustado.

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

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Indica que el texto se genera automáticamente.

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


Establece el modo de visualización del fondo

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indica si esta etiqueta de datos está eliminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Establece la dirección del texto.

Ver [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Establece la altura del marco en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.HeightRatioToChart, en su lugar. Height = HeightRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

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


Establece la altura del marco en unidades de la proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de proporción a píxeles? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

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

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Establece una referencia a la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


Indica si las etiquetas de datos nunca se superponen al generar una imagen de un gráfico circular. Nota: esta propiedad solo tiene sentido cuando se trata de un gráfico circular a imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Establece el formato numérico incorporado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Representa la cadena de formato para el objeto DataLabels.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Verdadero si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Representa la posición de la etiqueta de datos.

Ver [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Establece la posición del marco a automática

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. El ajuste automático ocurre cuando el texto dentro de una forma se escala para contener todo el texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representa el ángulo de rotación del texto.

**Remarks**


0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


Establece el tipo de separador usado para las etiquetas de datos en un gráfico.

Ver [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Para establecer un separador personalizado, establezca la propiedad [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) como [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) y luego especifique el valor esperado para [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


Establece el valor del separador usado para las etiquetas de datos en un gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


Establece el tipo de forma de la etiqueta de datos.

Ver [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor del porcentaje. False oculta el valor del porcentaje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado.True para mostrar el nombre de categoría de las etiquetas de datos en un gráfico. False para ocultar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


Indica si se muestra el rango de celdas como etiquetas de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. True si la clave de leyenda de la etiqueta de datos es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor del porcentaje. False oculta el valor del porcentaje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. True para mostrar el nombre de la serie. False para ocultar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. True muestra los valores. False para ocultar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece el texto de la etiqueta de datos.

**Remarks**

Solo funciona cuando esto es una etiqueta de datos de un punto de gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartTextFrame.ReadingOrder. Esta propiedad será eliminada 12 meses después desde marzo de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Establece la alineación horizontal del texto.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Establece la alineación vertical del texto.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Establece un valor que indica si el texto está ajustado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Establece el ancho del marco en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad ChartFrame.WidthRatioToChart, en su lugar. Width = WidthRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Establece el ancho del marco en unidades de proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de razón a píxeles? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.XRatioToChart, en su lugar. X = XRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Establece la coordenada x de la esquina superior izquierda en unidades de proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de razón a píxeles? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.YRatioToChart, en su lugar. Y = YRatioToChart \* 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Establece la coordenada y de la esquina superior izquierda en unidades de la proporción del área del gráfico.

**Remarks**

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de razón a píxeles? YPixel = YRatioToChart \* Chart.ChartObject.Height;

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

