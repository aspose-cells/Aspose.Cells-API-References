---
title: "ErrorBar"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la barra de error de la serie de datos."
type: docs
url: /es/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

Representa la barra de error de la serie de datos.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("a1").putValue(2);
         cells.get("a2").putValue(5);
         cells.get("a3").putValue(3);
         cells.get("a4").putValue(6);
         cells.get("b1").putValue(4);
         cells.get("b2").putValue(3);
         cells.get("b3").putValue(6);
         cells.get("b4").putValue(7);
 
         cells.get("C1").putValue("Q1");
         cells.get("C2").putValue("Q2");
         cells.get("C3").putValue("Y1");
         cells.get("C4").putValue("Y2");
 
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 11, 0, 27, 10);
 
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:B4", true);
 
         chart.getNSeries().setCategoryData("C1:C4");
 
         for(int i = 0; i <chart.getNSeries().getCount(); i ++)
         {
         		Series aseries = chart.getNSeries().get(i);
         		aseries.getYErrorBar().setDisplayType(ErrorBarDisplayType.MINUS);
         		aseries.getYErrorBar().setType(ErrorBarType.FIXED_VALUE);
         		aseries.getYErrorBar().setAmount(5);
         }
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Representa la cantidad de barra de error. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [getBeginType()](#getBeginType--) | Especifica una punta de flecha para el inicio de una línea. |
| [getCapType()](#getCapType--) | Especifica los extremos finales. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Representa el [Color](../../com.aspose.cells/color) de la línea. |
| [getCompoundType()](#getCompoundType--) | Especifica el tipo de línea compuesta |
| [getDashType()](#getDashType--) | Especifica el tipo de línea punteada |
| [getDisplayType()](#getDisplayType--) | Representa el tipo de visualización de la barra de error. |
| [getEndArrowLength()](#getEndArrowLength--) | Especifica la longitud de la punta de flecha para el extremo de una línea. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Especifica el ancho de la punta de flecha para el extremo de una línea. |
| [getEndType()](#getEndType--) | Especifica una punta de flecha para el extremo de una línea. |
| [getFormattingType()](#getFormattingType--) | Obtiene el tipo de formato. |
| [getGradientFill()](#getGradientFill--) | Representa el relleno degradado. |
| [getJoinType()](#getJoinType--) | Especifica los extremos de unión. |
| [getMinusValue()](#getMinusValue--) | Representa la cantidad de error negativo cuando el tipo de barra de error es Personalizado. |
| [getPlusValue()](#getPlusValue--) | Representa la cantidad de error positivo cuando el tipo de barra de error es Personalizado. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Indica si se formatean las barras de error con una T en la parte superior. |
| [getStyle()](#getStyle--) | Representa el estilo de la línea. |
| [getThemeColor()](#getThemeColor--) | Obtiene el color del tema. |
| [getTransparency()](#getTransparency--) | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro). |
| [getType()](#getType--) | Representa el tipo de cantidad de la barra de error. |
| [getWeight()](#getWeight--) | Obtiene el [WeightType](../../com.aspose.cells/weighttype) de la línea. |
| [getWeightPt()](#getWeightPt--) | Obtiene el grosor de la línea en unidades de puntos. |
| [getWeightPx()](#getWeightPx--) | Obtiene el peso de la línea en unidades de píxeles. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indica si este estilo de línea se asigna automáticamente. |
| [isAutomaticColor()](#isAutomaticColor--) | Indica si el color de la línea se asigna automáticamente. |
| [isVisible()](#isVisible--) | Representa si la línea es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | Representa la cantidad de barra de error. |
| [setAuto(boolean value)](#setAuto-boolean-) | Indica si este estilo de línea se asigna automáticamente. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [setBeginType(int value)](#setBeginType-int-) | Especifica una punta de flecha para el inicio de una línea. |
| [setCapType(int value)](#setCapType-int-) | Especifica los extremos finales. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Representa el [Color](../../com.aspose.cells/color) de la línea. |
| [setCompoundType(int value)](#setCompoundType-int-) | Especifica el tipo de línea compuesta |
| [setDashType(int value)](#setDashType-int-) | Especifica el tipo de línea punteada |
| [setDisplayType(int value)](#setDisplayType-int-) | Representa el tipo de visualización de la barra de error. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Especifica la longitud de la punta de flecha para el extremo de una línea. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Especifica el ancho de la punta de flecha para el extremo de una línea. |
| [setEndType(int value)](#setEndType-int-) | Especifica una punta de flecha para el extremo de una línea. |
| [setFormattingType(int value)](#setFormattingType-int-) | Establece el tipo de formato. |
| [setJoinType(int value)](#setJoinType-int-) | Especifica los extremos de unión. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | Representa la cantidad de error negativo cuando el tipo de barra de error es Personalizado. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | Representa la cantidad de error positivo cuando el tipo de barra de error es Personalizado. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | Indica si se formatean las barras de error con una T en la parte superior. |
| [setStyle(int value)](#setStyle-int-) | Representa el estilo de la línea. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Establece el color del tema. |
| [setTransparency(double value)](#setTransparency-double-) | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro). |
| [setType(int value)](#setType-int-) | Representa el tipo de cantidad de la barra de error. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


Representa la cantidad de barra de error.

**Remarks**

La cantidad debe ser mayor o igual que cero.

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
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


Representa el tipo de visualización de la barra de error.

Ver [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


Representa la cantidad de error negativo cuando el tipo de barra de error es Personalizado.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


Representa la cantidad de error positivo cuando el tipo de barra de error es Personalizado.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


Indica si se formatean las barras de error con una T en la parte superior.

**Returns:**
boolean
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


Representa el tipo de cantidad de la barra de error.

Ver [ErrorBarType](../../com.aspose.cells/errorbartype).

**Example**

```
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         Series aseries = chart.getNSeries().get(0);
         //Gets custom error bar type
         /*ErrorBarType*/int errBarType = aseries.getYErrorBar().getType();
         //Sets custom error bar type
         aseries.getYErrorBar().setType(ErrorBarType.CUSTOM);
         aseries.getYErrorBar().setPlusValue("=Sheet1!A1");
         aseries.getYErrorBar().setMinusValue("=Sheet1!A2");
```

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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


Representa la cantidad de barra de error.

**Remarks**

La cantidad debe ser mayor o igual que cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

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

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


Representa el tipo de visualización de la barra de error.

Ver [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


Representa la cantidad de error negativo cuando el tipo de barra de error es Personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


Representa la cantidad de error positivo cuando el tipo de barra de error es Personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


Indica si se formatean las barras de error con una T en la parte superior.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Representa el tipo de cantidad de la barra de error.

Ver [ErrorBarType](../../com.aspose.cells/errorbartype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

