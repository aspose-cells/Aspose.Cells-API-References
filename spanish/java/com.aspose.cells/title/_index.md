---
title: "Title"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa el título del gráfico o del eje."
type: docs
url: /es/java/com.aspose.cells/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Title extends ChartTextFrame
```

Encapsula el objeto que representa el título del gráfico o del eje.

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
         	Chart chart = sheet.getCharts().get(chartIndex);
 
         //Setting the title of a chart
         chart.getTitle().setText("Title");
         //Setting the font color of the chart title to blue
         chart.getTitle().getFont().setColor(Color.getBlue());
         //Setting the title of category axis of the chart
         chart.getCategoryAxis().getTitle().setText("Category");
         //Setting the title of value axis of the chart
         chart.getValueAxis().getTitle().setText("Value");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [characters()](#characters--) | Obtiene el formato de texto enriquecido de este Título. |
| [characters(int startIndex, int length)](#characters-int-int-) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtiene el [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [getBackground()](#getBackground--) | Obtiene el modo de visualización del fondo. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtiene el modo de visualización del fondo. |
| [getBorder()](#getBorder--) | Obtiene el [Line](../../com.aspose.cells/line). |
| [getCharacters()](#getCharacters--) | Obtiene el formato de texto enriquecido de este Título. |
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
| [getFont()](#getFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado. |
| [getHeight()](#getHeight--) | Obtiene la altura del marco en unidades de 1/4000 del área del gráfico. |
| [getHeightPixel()](#getHeightPixel--) | Obtiene la altura del marco en unidades de píxeles. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Obtiene la altura del marco en unidades de la proporción del área del gráfico. |
| [getLinkedSource()](#getLinkedSource--) | Obtiene una referencia a la hoja de cálculo. |
| [getOverLay()](#getOverLay--) | Representa un título superpuesto centrado en un gráfico sin cambiar el tamaño del gráfico. |
| [getReadingOrder()](#getReadingOrder--) | Representa el orden de lectura del texto. |
| [getRotationAngle()](#getRotationAngle--) | Representa el ángulo de rotación del texto. |
| [getShadow()](#getShadow--) | Verdadero si el marco tiene una sombra. |
| [getShapeProperties()](#getShapeProperties--) | Obtiene el objeto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getText()](#getText--) | Obtiene el texto de la etiqueta de unidad de visualización. |
| [getTextDirection()](#getTextDirection--) | Representa el orden de lectura del texto. |
| [getTextFont()](#getTextFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtiene la alineación horizontal del texto. |
| [getTextOptions()](#getTextOptions--) | Obtiene las opciones del texto. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtiene la alineación vertical del texto. |
| [getWidth()](#getWidth--) | Obtiene el ancho del marco en unidades de 1/4000 del área del gráfico. |
| [getWidthPixel()](#getWidthPixel--) | Obtiene el ancho del marco en unidades de píxel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Obtiene el ancho del marco en unidades de la proporción del área del gráfico. |
| [getX()](#getX--) | Obtiene la coordenada X de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [getXPixel()](#getXPixel--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de píxel. |
| [getXRatioToChart()](#getXRatioToChart--) | Obtiene la coordenada x de la esquina superior izquierda en unidades de Fracción del área del gráfico. |
| [getY()](#getY--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [getYPixel()](#getYPixel--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles. |
| [getYRatioToChart()](#getYRatioToChart--) | Obtiene la coordenada y de la esquina superior izquierda en unidades de Fracción del área del gráfico. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indica que el texto se genera automáticamente. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indica si el texto del gráfico se rota automáticamente. |
| [isAutomaticSize()](#isAutomaticSize--) | Indica si el marco del gráfico tiene tamaño automático. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida. |
| [isDeleted()](#isDeleted--) | Indica si esta etiqueta de datos está eliminada. |
| [isInnerMode()](#isInnerMode--) | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Obtiene si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. |
| [isTextWrapped()](#isTextWrapped--) | Obtiene un valor que indica si el texto está ajustado. |
| [isVisible()](#isVisible--) | Representa si el título es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indica que el texto se genera automáticamente. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indica si el marco del gráfico tiene tamaño automático. |
| [setBackground(int value)](#setBackground-int-) | Establece el modo de visualización del fondo. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Establece el modo de visualización del fondo. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indica si esta etiqueta de datos está eliminada. |
| [setDirectionType(int value)](#setDirectionType-int-) | Establece la dirección del texto. |
| [setHeight(int value)](#setHeight-int-) | Establece la altura del marco en unidades de 1/4000 del área del gráfico. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Establece la altura del marco en unidades de píxeles. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Establece la altura del marco en unidades de la proporción del área del gráfico. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Establece una referencia a la hoja de cálculo. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Representa un título superpuesto centrado en un gráfico sin cambiar el tamaño del gráfico. |
| [setPositionAuto()](#setPositionAuto--) | Establece la posición del marco a automática |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Representa el orden de lectura del texto. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representa el ángulo de rotación del texto. |
| [setShadow(boolean value)](#setShadow-boolean-) | Verdadero si el marco tiene una sombra. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto de la etiqueta de unidad de visualización. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representa el orden de lectura del texto. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Establece la alineación horizontal del texto. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Establece la alineación vertical del texto. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Establece un valor que indica si el texto está ajustado. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representa si el título es visible. |
| [setWidth(int value)](#setWidth-int-) | Establece el ancho del marco en unidades de 1/4000 del área del gráfico. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Establece el ancho del marco en unidades de píxel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Establece el ancho del marco en unidades de proporción del área del gráfico. |
| [setX(int value)](#setX-int-) | Establece la coordenada X de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [setXPixel(int value)](#setXPixel-int-) | Establece la coordenada x de la esquina superior izquierda en unidades de píxel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Establece la coordenada x de la esquina superior izquierda en unidades de fracción del área del gráfico. |
| [setY(int value)](#setY-int-) | Establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| [setYPixel(int value)](#setYPixel-int-) | Establece la coordenada y de la esquina superior izquierda en unidades de píxeles. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Establece la coordenada y de la esquina superior izquierda en unidades de fracción del área del gráfico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters() {#characters--}
```
public FontSetting[] characters()
```


Obtiene el formato de texto enriquecido de este Título.

**Returns:**
com.aspose.cells.FontSetting[] - devuelve una matriz de FontSetting
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
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Obtiene el formato de texto enriquecido de este Título.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Title.Characters(). Esta propiedad será eliminada 12 meses después a partir de noviembre de 2016. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
com.aspose.cells.FontSetting[] - devuelve una matriz de FontSetting
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


Obtiene un objeto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del objeto ChartFrame especificado.

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
### getOverLay() {#getOverLay--}
```
public boolean getOverLay()
```


Representa un título superpuesto centrado en un gráfico sin cambiar el tamaño del gráfico.

**Returns:**
boolean
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
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto de la etiqueta de unidad de visualización.

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


Obtiene la coordenada X de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad Title.XRatioToChart, en su lugar. X = XRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Obtiene la coordenada x de la esquina superior izquierda en unidades de fracción del área del gráfico. X en píxeles = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad Title.YRatioToChart, en su lugar. Y = YRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Obtiene la coordenada y de la esquina superior izquierda en unidades de fracción del área del gráfico. Y en píxeles = YRatioToChart \* Chart.ChartObject.Width;

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
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representa si el título es visible.

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


Establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

Ver [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de febrero de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

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

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Representa un título superpuesto centrado en un gráfico sin cambiar el tamaño del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece el texto de la etiqueta de unidad de visualización.

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

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representa si el título es visible.

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


Establece la coordenada X de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

**Remarks**

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad Title.XRatioToChart, en su lugar. X = XRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Establece la coordenada x de la esquina superior izquierda en unidades de fracción del área del gráfico. X en píxeles = XRatioToChart \* Chart.ChartObject.Width;

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

NOTA: Este miembro está ahora obsoleto. Utilice la propiedad Title.YRatioToChart, en su lugar. Y = YRatioToChart \* 4000; Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


Establece la coordenada y de la esquina superior izquierda en unidades de fracción del área del gráfico. Y en píxeles = YRatioToChart \* Chart.ChartObject.Width;

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

