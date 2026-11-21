---
title: "Duvarlar"
second_title: "Aspose.Cells for Java API Referansı"
description: "3D grafik duvarlarını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/walls/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area), [com.aspose.cells.Floor](../../com.aspose.cells/floor)
```
public class Walls extends Floor
```

3D grafik duvarlarını temsil eden nesneyi kapsüller.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | [Area](../../com.aspose.cells/area) öğesinin arka plan [Color](../../com.aspose.cells/color) değerini alır. |
| [getBorder()](#getBorder--) | Kenarı [Line](../../com.aspose.cells/line) alır. |
| [getCenterX()](#getCenterX--) | Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin x koordinatını, grafiğin genişliğinin 1/4000'i biriminde alır. |
| [getCenterXPx()](#getCenterXPx--) | Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin x koordinatını piksel biriminde alır. |
| [getCenterY()](#getCenterY--) | Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin y koordinatını, grafiğin yüksekliğinin 1/4000'i biriminde alır. |
| [getCenterYPx()](#getCenterYPx--) | Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin y koordinatını piksel biriminde alır. |
| [getClass()](#getClass--) |  |
| [getCubePointCount()](#getCubePointCount--) | Chart.Calculate() metodunu çağırdıktan sonra, küp noktalarının sayısını alır. |
| [getCubePointXPx(int index)](#getCubePointXPx-int-) | Chart.Calculate() metodunu çağırdıktan sonra, duvar küpünün tepe noktasının x koordinatını alır. |
| [getCubePointYPx(int index)](#getCubePointYPx-int-) | Chart.Calculate() metodunu çağırdıktan sonra, duvar küpünün tepe noktasının y koordinatını alır. |
| [getDepth()](#getDepth--) | Chart.Calculate() metodunu çağırdıktan sonra, grafiğin genişliğinin 1/4000'i biriminde, ön‑ark derinliğini alır. |
| [getDepthPx()](#getDepthPx--) | Chart.Calculate() metodunu çağırdıktan sonra, ön‑ark derinliğini piksel biriminde alır. |
| [getFillFormat()](#getFillFormat--) | Belirtilen grafik veya şekil için dolgu biçimlendirme özelliklerini içeren bir [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) nesnesini temsil eder. |
| [getForegroundColor()](#getForegroundColor--) | Ön plan [Color](../../com.aspose.cells/color) değerini alır. |
| [getFormatting()](#getFormatting--) | Alan biçimlendirmesini temsil eder. |
| [getHeight()](#getHeight--) | Chart.Calculate() metodunu çağırdıktan sonra, grafiğin yüksekliğinin 1/4000'i biriminde, üst‑alt yüksekliğini alır. |
| [getHeightPx()](#getHeightPx--) | Chart.Calculate() metodunu çağırdıktan sonra, üst‑alt yüksekliği piksel biriminde alır. |
| [getInvertIfNegative()](#getInvertIfNegative--) | Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir. |
| [getTransparency()](#getTransparency--) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [getWidth()](#getWidth--) | Chart.Calculate() metodunu çağırdıktan sonra, grafiğin genişliğinin 1/4000'i biriminde, sol‑sağ genişliğini alır. |
| [getWidthPx()](#getWidthPx--) | Chart.Calculate() metodunu çağırdıktan sonra, sol‑sağ genişliği piksel biriminde alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | [Area](../../com.aspose.cells/area) öğesinin arka plan [Color](../../com.aspose.cells/color) değerini ayarlar. |
| [setBorder(Line value)](#setBorder-com.aspose.cells.Line-) | Kenarı [Line](../../com.aspose.cells/line) ayarlar. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Ön plan [Color](../../com.aspose.cells/color) değerini ayarlar. |
| [setFormatting(int value)](#setFormatting-int-) | Alan biçimlendirmesini temsil eder. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir. |
| [setTransparency(double value)](#setTransparency-double-) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


[Area](../../com.aspose.cells/area) öğesinin arka plan [Color](../../com.aspose.cells/color) değerini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Kenarı [Line](../../com.aspose.cells/line) alır.

**Returns:**
[Line](../../com.aspose.cells/line)
### getCenterX() {#getCenterX--}
```
public int getCenterX()
```


Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin x koordinatını, grafiğin genişliğinin 1/4000'i biriminde alır.

**Returns:**
int
### getCenterXPx() {#getCenterXPx--}
```
public int getCenterXPx()
```


Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin x koordinatını piksel biriminde alır.

**Returns:**
int
### getCenterY() {#getCenterY--}
```
public int getCenterY()
```


Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin y koordinatını, grafiğin yüksekliğinin 1/4000'i biriminde alır.

**Returns:**
int
### getCenterYPx() {#getCenterYPx--}
```
public int getCenterYPx()
```


Chart.Calculate() metodunu çağırdıktan sonra, duvar merkezinin sol‑alt köşesinin y koordinatını piksel biriminde alır.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCubePointCount() {#getCubePointCount--}
```
public int getCubePointCount()
```


Chart.Calculate() metodunu çağırdıktan sonra, küp noktalarının sayısını alır.

**Returns:**
int
### getCubePointXPx(int index) {#getCubePointXPx-int-}
```
public float getCubePointXPx(int index)
```


Chart.Calculate() metodunu çağırdıktan sonra, duvar küpünün tepe noktasının x koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getCubePointYPx(int index) {#getCubePointYPx-int-}
```
public float getCubePointYPx(int index)
```


Chart.Calculate() metodunu çağırdıktan sonra, duvar küpünün tepe noktasının y koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getDepth() {#getDepth--}
```
public int getDepth()
```


Chart.Calculate() metodunu çağırdıktan sonra, grafiğin genişliğinin 1/4000'i biriminde, ön‑ark derinliğini alır.

**Returns:**
int
### getDepthPx() {#getDepthPx--}
```
public int getDepthPx()
```


Chart.Calculate() metodunu çağırdıktan sonra, ön‑ark derinliğini piksel biriminde alır.

**Returns:**
int
### getFillFormat() {#getFillFormat--}
```
public FillFormat getFillFormat()
```


Belirtilen grafik veya şekil için dolgu biçimlendirme özelliklerini içeren bir [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) nesnesini temsil eder.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Ön plan [Color](../../com.aspose.cells/color) değerini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


Alan biçimlendirmesini temsil eder.

[FormattingType](../../com.aspose.cells/formattingtype) bölümüne bakın.

**Returns:**
int
### getHeight() {#getHeight--}
```
public int getHeight()
```


Chart.Calculate() metodunu çağırdıktan sonra, grafiğin yüksekliğinin 1/4000'i biriminde, üst‑alt yüksekliğini alır.

**Returns:**
int
### getHeightPx() {#getHeightPx--}
```
public int getHeightPx()
```


Chart.Calculate() metodunu çağırdıktan sonra, üst‑alt yüksekliği piksel biriminde alır.

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(-100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
         chart.getNSeries().add("A1:A3", true);
         boolean isNegative = chart.getNSeries().get(0).getArea().getInvertIfNegative();
         chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
         //Setting the foreground color of the 1st NSeries area
         chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed());
         //Setting the background color of the 1st NSeries area.
         //The displayed area color of second chart point will be the background color.
         chart.getNSeries().get(0).getArea().setBackgroundColor(Color.getYellow());
         //Saving the Excel file
         workbook.save("book1.xls");
```

**Returns:**
boolean
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Returns:**
double
### getWidth() {#getWidth--}
```
public int getWidth()
```


Chart.Calculate() metodunu çağırdıktan sonra, grafiğin genişliğinin 1/4000'i biriminde, sol‑sağ genişliğini alır.

**Returns:**
int
### getWidthPx() {#getWidthPx--}
```
public int getWidthPx()
```


Chart.Calculate() metodunu çağırdıktan sonra, sol‑sağ genişliği piksel biriminde alır.

**Returns:**
int
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




### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


[Area](../../com.aspose.cells/area) öğesinin arka plan [Color](../../com.aspose.cells/color) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBorder(Line value) {#setBorder-com.aspose.cells.Line-}
```
public void setBorder(Line value)
```


Kenarı [Line](../../com.aspose.cells/line) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Line](../../com.aspose.cells/line) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Ön plan [Color](../../com.aspose.cells/color) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


Alan biçimlendirmesini temsil eder.

[FormattingType](../../com.aspose.cells/formattingtype) bölümüne bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

