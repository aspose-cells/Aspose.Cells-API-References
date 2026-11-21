---
title: "Çizgi"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çizgi biçimini temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

Çizgi biçimini temsil eden nesneyi kapsar.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | Bir çizginin başlangıcı için ok başının uzunluğunu belirtir. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Bir çizginin başlangıcı için ok başının genişliğini belirtir. |
| [getBeginType()](#getBeginType--) | Bir çizginin başlangıcı için bir ok başı belirtir. |
| [getCapType()](#getCapType--) | Bitiş kapaklarını belirtir. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Satırın [Color](../../com.aspose.cells/color) değerini temsil eder. |
| [getCompoundType()](#getCompoundType--) | Bileşik çizgi tipini belirtir |
| [getDashType()](#getDashType--) | Kesikli çizgi tipini belirtir |
| [getEndArrowLength()](#getEndArrowLength--) | Bir çizginin ucundaki ok başının uzunluğunu belirtir. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Bir çizginin ucundaki ok başının genişliğini belirtir. |
| [getEndType()](#getEndType--) | Bir çizginin ucunda bir ok başı belirtir. |
| [getFormattingType()](#getFormattingType--) | Biçim tipini alır. |
| [getGradientFill()](#getGradientFill--) | Gradyan doldurmayı temsil eder. |
| [getJoinType()](#getJoinType--) | Birleştirme kapaklarını belirtir. |
| [getStyle()](#getStyle--) | Çizginin stilini temsil eder. |
| [getThemeColor()](#getThemeColor--) | Tema rengini alır. |
| [getTransparency()](#getTransparency--) | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [getWeight()](#getWeight--) | Çizginin [WeightType](../../com.aspose.cells/weighttype) değerini alır. |
| [getWeightPt()](#getWeightPt--) | Çizginin ağırlığını puan biriminde alır. |
| [getWeightPx()](#getWeightPx--) | Satırın ağırlığını piksel biriminde alır. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir. |
| [isAutomaticColor()](#isAutomaticColor--) | Çizgi renginin otomatik olarak atanıp atanmadığını gösterir. |
| [isVisible()](#isVisible--) | Çizginin görünür olup olmadığını temsil eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Bir çizginin başlangıcı için ok başının uzunluğunu belirtir. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Bir çizginin başlangıcı için ok başının genişliğini belirtir. |
| [setBeginType(int value)](#setBeginType-int-) | Bir çizginin başlangıcı için bir ok başı belirtir. |
| [setCapType(int value)](#setCapType-int-) | Bitiş kapaklarını belirtir. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Satırın [Color](../../com.aspose.cells/color) değerini temsil eder. |
| [setCompoundType(int value)](#setCompoundType-int-) | Bileşik çizgi tipini belirtir |
| [setDashType(int value)](#setDashType-int-) | Kesikli çizgi tipini belirtir |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Bir çizginin ucundaki ok başının uzunluğunu belirtir. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Bir çizginin ucundaki ok başının genişliğini belirtir. |
| [setEndType(int value)](#setEndType-int-) | Bir çizginin ucunda bir ok başı belirtir. |
| [setFormattingType(int value)](#setFormattingType-int-) | Biçim türünü ayarlar. |
| [setJoinType(int value)](#setJoinType-int-) | Birleştirme kapaklarını belirtir. |
| [setStyle(int value)](#setStyle-int-) | Çizginin stilini temsil eder. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Tema rengini ayarlar. |
| [setTransparency(double value)](#setTransparency-double-) | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Çizginin görünür olup olmadığını temsil eder. |
| [setWeight(int value)](#setWeight-int-) | Satırın [WeightType](../../com.aspose.cells/weighttype) değerini ayarlar. |
| [setWeightPt(double value)](#setWeightPt-double-) | Satırın ağırlığını nokta biriminde ayarlar. |
| [setWeightPx(double value)](#setWeightPx-double-) | Satırın ağırlığını piksel biriminde ayarlar. |
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
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Bir çizginin başlangıcı için ok başının uzunluğunu belirtir.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Bir çizginin başlangıcı için ok başının genişliğini belirtir.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Bir çizginin başlangıcı için bir ok başı belirtir.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Bitiş kapaklarını belirtir.

Bakınız [LineCapType](../../com.aspose.cells/linecaptype).

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


Satırın [Color](../../com.aspose.cells/color) değerini temsil eder.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Bileşik çizgi tipini belirtir

Bakınız [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Kesikli çizgi tipini belirtir

Bakınız [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Bir çizginin ucundaki ok başının uzunluğunu belirtir.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Bir çizginin ucundaki ok başının genişliğini belirtir.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Bir çizginin ucunda bir ok başı belirtir.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Biçim tipini alır.

Bakınız [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Gradyan doldurmayı temsil eder.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Birleştirme kapaklarını belirtir.

Bakınız [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Çizginin stilini temsil eder.

Bakın [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Tema rengini alır.

**Remarks**

Ön plan rengi bir tema rengi değilse, NULL döndürülecektir.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Returns:**
double
### getWeight() {#getWeight--}
```
public int getWeight()
```


Çizginin [WeightType](../../com.aspose.cells/weighttype) değerini alır.

Bakın [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Çizginin ağırlığını puan biriminde alır.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Satırın ağırlığını piksel biriminde alır.

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


Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Çizgi renginin otomatik olarak atanıp atanmadığını gösterir.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Çizginin görünür olup olmadığını temsil eder.

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


Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Bir çizginin başlangıcı için ok başının uzunluğunu belirtir.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Bir çizginin başlangıcı için ok başının genişliğini belirtir.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Bir çizginin başlangıcı için bir ok başı belirtir.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Bitiş kapaklarını belirtir.

Bakınız [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Satırın [Color](../../com.aspose.cells/color) değerini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Bileşik çizgi tipini belirtir

Bakınız [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Kesikli çizgi tipini belirtir

Bakınız [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Bir çizginin ucundaki ok başının uzunluğunu belirtir.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Bir çizginin ucundaki ok başının genişliğini belirtir.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Bir çizginin ucunda bir ok başı belirtir.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Biçim türünü ayarlar.

Bakınız [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Birleştirme kapaklarını belirtir.

Bakınız [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Çizginin stilini temsil eder.

Bakın [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Tema rengini ayarlar.

**Remarks**

Ön plan rengi bir tema rengi değilse, NULL döndürülecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Çizginin görünür olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Satırın [WeightType](../../com.aspose.cells/weighttype) değerini ayarlar.

Bakın [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Satırın ağırlığını nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Satırın ağırlığını piksel biriminde ayarlar.

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

