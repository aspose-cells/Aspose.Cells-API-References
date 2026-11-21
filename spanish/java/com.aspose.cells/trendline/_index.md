---
title: "Trendline"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una línea de tendencia en un gráfico."
type: docs
url: /es/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Representa una línea de tendencia en un gráfico.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [getBeginType()](#getBeginType--) | Especifica una punta de flecha para el inicio de una línea. |
| [getCapType()](#getCapType--) | Especifica los extremos finales. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Representa el [Color](../../com.aspose.cells/color) de la línea. |
| [getCompoundType()](#getCompoundType--) | Especifica el tipo de línea compuesta |
| [getDashType()](#getDashType--) | Especifica el tipo de línea punteada |
| [getDataLabels()](#getDataLabels--) | Representa el objeto DataLabels para la serie especificada. |
| [getDisplayEquation()](#getDisplayEquation--) | Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor R al cuadrado). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Representa si el valor R al cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). |
| [getEndArrowLength()](#getEndArrowLength--) | Especifica la longitud de la punta de flecha para el extremo de una línea. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Especifica el ancho de la punta de flecha para el extremo de una línea. |
| [getEndType()](#getEndType--) | Especifica una punta de flecha para el extremo de una línea. |
| [getFormattingType()](#getFormattingType--) | Obtiene el tipo de formato. |
| [getForward()](#getForward--) | Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. |
| [getGradientFill()](#getGradientFill--) | Representa el relleno degradado. |
| [getIntercept()](#getIntercept--) | Devuelve o establece el punto donde la línea de tendencia cruza el eje de valores. |
| [getJoinType()](#getJoinType--) | Especifica los extremos de unión. |
| [getLegendEntry()](#getLegendEntry--) | Obtiene la entrada de leyenda según esta línea de tendencia |
| [getName()](#getName--) | Devuelve el nombre de la línea de tendencia. |
| [getOrder()](#getOrder--) | Devuelve o establece el orden de la línea de tendencia (un entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. |
| [getPeriod()](#getPeriod--) | Devuelve o establece el período para la línea de tendencia de media móvil. |
| [getStyle()](#getStyle--) | Representa el estilo de la línea. |
| [getThemeColor()](#getThemeColor--) | Obtiene el color del tema. |
| [getTransparency()](#getTransparency--) | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro). |
| [getType()](#getType--) | Devuelve el tipo de línea de tendencia. |
| [getWeight()](#getWeight--) | Obtiene el [WeightType](../../com.aspose.cells/weighttype) de la línea. |
| [getWeightPt()](#getWeightPt--) | Obtiene el grosor de la línea en unidades de puntos. |
| [getWeightPx()](#getWeightPx--) | Obtiene el peso de la línea en unidades de píxeles. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indica si este estilo de línea se asigna automáticamente. |
| [isAutomaticColor()](#isAutomaticColor--) | Indica si el color de la línea se asigna automáticamente. |
| [isInterceptAuto()](#isInterceptAuto--) | Indica si Microsoft Workbook determina automáticamente la intersección de la línea de tendencia. |
| [isNameAuto()](#isNameAuto--) | Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia. |
| [isVisible()](#isVisible--) | Representa si la línea es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indica si este estilo de línea se asigna automáticamente. |
| [setBackward(double value)](#setBackward-double-) | Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [setBeginType(int value)](#setBeginType-int-) | Especifica una punta de flecha para el inicio de una línea. |
| [setCapType(int value)](#setCapType-int-) | Especifica los extremos finales. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Representa el [Color](../../com.aspose.cells/color) de la línea. |
| [setCompoundType(int value)](#setCompoundType-int-) | Especifica el tipo de línea compuesta |
| [setDashType(int value)](#setDashType-int-) | Especifica el tipo de línea punteada |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor R al cuadrado). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Representa si el valor R al cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Especifica la longitud de la punta de flecha para el extremo de una línea. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Especifica el ancho de la punta de flecha para el extremo de una línea. |
| [setEndType(int value)](#setEndType-int-) | Especifica una punta de flecha para el extremo de una línea. |
| [setFormattingType(int value)](#setFormattingType-int-) | Establece el tipo de formato. |
| [setForward(double value)](#setForward-double-) | Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. |
| [setIntercept(double value)](#setIntercept-double-) | Devuelve o establece el punto donde la línea de tendencia cruza el eje de valores. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Establece si Microsoft Workbook determina automáticamente la intersección de la línea de tendencia. |
| [setJoinType(int value)](#setJoinType-int-) | Especifica los extremos de unión. |
| [setName(String value)](#setName-java.lang.String-) | Devuelve el nombre de la línea de tendencia. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia. |
| [setOrder(int value)](#setOrder-int-) | Devuelve o establece el orden de la línea de tendencia (un entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. |
| [setPeriod(int value)](#setPeriod-int-) | Devuelve o establece el período para la línea de tendencia de media móvil. |
| [setStyle(int value)](#setStyle-int-) | Representa el estilo de la línea. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Establece el color del tema. |
| [setTransparency(double value)](#setTransparency-double-) | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro). |
| [setVisible(boolean value)](#setVisible-boolean-) | Representa si la línea es visible. |
| [setWeight(int value)](#setWeight-int-) | Establece el [WeightType](../../com.aspose.cells/weighttype) de la línea. |
| [setWeightPt(double value)](#setWeightPt-double-) | Establece el peso de la línea en unidades de puntos. |
| [setWeightPx(double value)](#setWeightPx-double-) | Establece el peso de la línea en unidades de píxeles. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. El número de períodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de períodos debe estar entre 0 y 0,5.

**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Especifica la longitud de la punta de flecha para el inicio de una línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Especifica el ancho de la punta de flecha para el inicio de una línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Especifica una punta de flecha para el inicio de una línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Especifica los extremos finales.

Ver [LineCapType](../../com.aspose.cells/linecaptype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Representa el [Color](../../com.aspose.cells/color) de la línea.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Especifica el tipo de línea compuesta

Ver [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Especifica el tipo de línea punteada

Ver [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Representa el objeto DataLabels para la serie especificada.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor de R al cuadrado). Establecer esta propiedad en True activa automáticamente las etiquetas de datos.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Representa si el valor de R al cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). Establecer esta propiedad en True activa automáticamente las etiquetas de datos.

**Returns:**
boolean
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Especifica la longitud de la punta de flecha para el extremo de una línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Especifica el ancho de la punta de flecha para el extremo de una línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Especifica una punta de flecha para el extremo de una línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Obtiene el tipo de formato.

Ver [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getForward() {#getForward--}
```
public double getForward()
```


Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Representa el relleno degradado.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Devuelve o establece el punto donde la línea de tendencia cruza el eje de valores.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Especifica los extremos de unión.

Ver [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Obtiene la entrada de leyenda según esta línea de tendencia

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Devuelve el nombre de la línea de tendencia.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Devuelve o establece el orden de la línea de tendencia (un entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. El orden debe estar entre 2 y 6.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Devuelve o establece el período para la línea de tendencia de media móvil.

**Remarks**

Este valor debe estar entre 2 y 255. Y debe ser menor que el número de puntos del gráfico en la serie

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Representa el estilo de la línea.

Ver [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtiene el color del tema.

**Remarks**

Si el color de primer plano no es un color de tema, se devolverá NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Devuelve el tipo de línea de tendencia.

Ver [TrendlineType](../../com.aspose.cells/trendlinetype).

**Returns:**
int
### getWeight() {#getWeight--}
```
public int getWeight()
```


Obtiene el [WeightType](../../com.aspose.cells/weighttype) de la línea.

Ver [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Obtiene el grosor de la línea en unidades de puntos.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Obtiene el peso de la línea en unidades de píxeles.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


Indica si este estilo de línea se asigna automáticamente.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Indica si el color de la línea se asigna automáticamente.

**Returns:**
boolean
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Indica si Microsoft Workbook determina automáticamente la intersección de la línea de tendencia.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representa si la línea es visible.

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Indica si este estilo de línea se asigna automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. El número de períodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de períodos debe estar entre 0 y 0,5.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Especifica la longitud de la punta de flecha para el inicio de una línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Especifica el ancho de la punta de flecha para el inicio de una línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Especifica una punta de flecha para el inicio de una línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Especifica los extremos finales.

Ver [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Representa el [Color](../../com.aspose.cells/color) de la línea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Especifica el tipo de línea compuesta

Ver [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Especifica el tipo de línea punteada

Ver [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor de R al cuadrado). Establecer esta propiedad en True activa automáticamente las etiquetas de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Representa si el valor de R al cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). Establecer esta propiedad en True activa automáticamente las etiquetas de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Especifica la longitud de la punta de flecha para el extremo de una línea.

Ver [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Especifica el ancho de la punta de flecha para el extremo de una línea.

Ver [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Especifica una punta de flecha para el extremo de una línea.

Ver [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Establece el tipo de formato.

Ver [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Devuelve o establece el punto donde la línea de tendencia cruza el eje de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Establece si Microsoft Workbook determina automáticamente la intersección de la línea de tendencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Especifica los extremos de unión.

Ver [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Devuelve el nombre de la línea de tendencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Devuelve o establece el orden de la línea de tendencia (un entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. El orden debe estar entre 2 y 6.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Devuelve o establece el período para la línea de tendencia de media móvil.

**Remarks**

Este valor debe estar entre 2 y 255. Y debe ser menor que el número de puntos del gráfico en la serie

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Representa el estilo de la línea.

Ver [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Establece el color del tema.

**Remarks**

Si el color de primer plano no es un color de tema, se devolverá NULL.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representa si la línea es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Establece el [WeightType](../../com.aspose.cells/weighttype) de la línea.

Ver [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Establece el peso de la línea en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Establece el peso de la línea en unidades de píxeles.

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

