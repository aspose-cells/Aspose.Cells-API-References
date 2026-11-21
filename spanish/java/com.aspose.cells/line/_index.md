---
title: "Line"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa el formato de línea."
type: docs
url: /es/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

Encapsula el objeto que representa el formato de línea.

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
 
         	int chartIndex = sheet.getCharts().add(ChartType.LINE, 9, 9, 21, 15);
         Chart chart = sheet.getCharts().get(chartIndex);
         //Add series
         chart.getNSeries().add("A2:B4", true);
         //Set category data
         chart.getNSeries().setCategoryData("=Sheet1!$A$2:$A$4");
         //Applying a dotted line style on the lines of an NSeries
         chart.getNSeries().get(0).getBorder().setStyle(LineType.DOT);
         chart.getNSeries().get(0).getBorder().setColor(Color.getRed());
         //Applying a triangular marker style on the data markers of an NSeries
         chart.getNSeries().get(0).getMarker().setMarkerStyle(ChartMarkerType.TRIANGLE);
         //Setting the weight of all lines in an NSeries to medium
         chart.getNSeries().get(0).getBorder().setWeight(WeightType.MEDIUM_LINE);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [getBeginType()](#getBeginType--) | Especifica una punta de flecha para el inicio de una línea. |
| [getCapType()](#getCapType--) | Especifica los extremos finales. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Representa el [Color](../../com.aspose.cells/color) de la línea. |
| [getCompoundType()](#getCompoundType--) | Especifica el tipo de línea compuesta |
| [getDashType()](#getDashType--) | Especifica el tipo de línea punteada |
| [getEndArrowLength()](#getEndArrowLength--) | Especifica la longitud de la punta de flecha para el extremo de una línea. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Especifica el ancho de la punta de flecha para el extremo de una línea. |
| [getEndType()](#getEndType--) | Especifica una punta de flecha para el extremo de una línea. |
| [getFormattingType()](#getFormattingType--) | Obtiene el tipo de formato. |
| [getGradientFill()](#getGradientFill--) | Representa el relleno degradado. |
| [getJoinType()](#getJoinType--) | Especifica los extremos de unión. |
| [getStyle()](#getStyle--) | Representa el estilo de la línea. |
| [getThemeColor()](#getThemeColor--) | Obtiene el color del tema. |
| [getTransparency()](#getTransparency--) | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro). |
| [getWeight()](#getWeight--) | Obtiene el [WeightType](../../com.aspose.cells/weighttype) de la línea. |
| [getWeightPt()](#getWeightPt--) | Obtiene el grosor de la línea en unidades de puntos. |
| [getWeightPx()](#getWeightPx--) | Obtiene el peso de la línea en unidades de píxeles. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indica si este estilo de línea se asigna automáticamente. |
| [isAutomaticColor()](#isAutomaticColor--) | Indica si el color de la línea se asigna automáticamente. |
| [isVisible()](#isVisible--) | Representa si la línea es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indica si este estilo de línea se asigna automáticamente. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [setBeginType(int value)](#setBeginType-int-) | Especifica una punta de flecha para el inicio de una línea. |
| [setCapType(int value)](#setCapType-int-) | Especifica los extremos finales. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Representa el [Color](../../com.aspose.cells/color) de la línea. |
| [setCompoundType(int value)](#setCompoundType-int-) | Especifica el tipo de línea compuesta |
| [setDashType(int value)](#setDashType-int-) | Especifica el tipo de línea punteada |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Especifica la longitud de la punta de flecha para el extremo de una línea. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Especifica el ancho de la punta de flecha para el extremo de una línea. |
| [setEndType(int value)](#setEndType-int-) | Especifica una punta de flecha para el extremo de una línea. |
| [setFormattingType(int value)](#setFormattingType-int-) | Establece el tipo de formato. |
| [setJoinType(int value)](#setJoinType-int-) | Especifica los extremos de unión. |
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
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Representa el relleno degradado.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Especifica los extremos de unión.

Ver [LineJoinType](../../com.aspose.cells/linejointype).

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

