---
title: "Trendline"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir grafikteki eğriyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Bir grafikteki eğriyi temsil eder.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Trend çizgisinin geriye doğru uzandığı dönem (veya dağılım grafiğindeki birimler) sayısını döndürür veya ayarlar. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Bir çizginin başlangıcı için ok başının uzunluğunu belirtir. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Bir çizginin başlangıcı için ok başının genişliğini belirtir. |
| [getBeginType()](#getBeginType--) | Bir çizginin başlangıcı için bir ok başı belirtir. |
| [getCapType()](#getCapType--) | Bitiş kapaklarını belirtir. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Satırın [Color](../../com.aspose.cells/color) değerini temsil eder. |
| [getCompoundType()](#getCompoundType--) | Bileşik çizgi tipini belirtir |
| [getDashType()](#getDashType--) | Kesikli çizgi tipini belirtir |
| [getDataLabels()](#getDataLabels--) | Belirtilen seriye ait DataLabels nesnesini temsil eder. |
| [getDisplayEquation()](#getDisplayEquation--) | Trend çizgisinin denkleminin grafikte (R-kare değeriyle aynı veri etiketinde) gösterilip gösterilmediğini temsil eder. |
| [getDisplayRSquared()](#getDisplayRSquared--) | Trend çizgisinin R-kare değerinin grafikte (denklemin aynı veri etiketinde) gösterilip gösterilmediğini temsil eder. |
| [getEndArrowLength()](#getEndArrowLength--) | Bir çizginin ucundaki ok başının uzunluğunu belirtir. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Bir çizginin ucundaki ok başının genişliğini belirtir. |
| [getEndType()](#getEndType--) | Bir çizginin ucunda bir ok başı belirtir. |
| [getFormattingType()](#getFormattingType--) | Biçim tipini alır. |
| [getForward()](#getForward--) | Trend çizgisinin ileri doğru uzandığı dönem (veya dağılım grafiğindeki birim) sayısını alır veya ayarlar. |
| [getGradientFill()](#getGradientFill--) | Gradyan doldurmayı temsil eder. |
| [getIntercept()](#getIntercept--) | Trend çizgisinin değer eksenini kestiği noktayı alır veya ayarlar. |
| [getJoinType()](#getJoinType--) | Birleştirme kapaklarını belirtir. |
| [getLegendEntry()](#getLegendEntry--) | Bu trend çizgisine göre gösterge girişini alır. |
| [getName()](#getName--) | Trend çizgisinin adını döndürür. |
| [getOrder()](#getOrder--) | Trend çizgisi tipi Polinom olduğunda trend çizgisi derecesini (1'den büyük bir tam sayı) alır veya ayarlar. |
| [getPeriod()](#getPeriod--) | Hareketli ortalama trend çizgisi için periyodu alır veya ayarlar. |
| [getStyle()](#getStyle--) | Çizginin stilini temsil eder. |
| [getThemeColor()](#getThemeColor--) | Tema rengini alır. |
| [getTransparency()](#getTransparency--) | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [getType()](#getType--) | Trend çizgisi tipini döndürür. |
| [getWeight()](#getWeight--) | Çizginin [WeightType](../../com.aspose.cells/weighttype) değerini alır. |
| [getWeightPt()](#getWeightPt--) | Çizginin ağırlığını puan biriminde alır. |
| [getWeightPx()](#getWeightPx--) | Satırın ağırlığını piksel biriminde alır. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir. |
| [isAutomaticColor()](#isAutomaticColor--) | Çizgi renginin otomatik olarak atanıp atanmadığını gösterir. |
| [isInterceptAuto()](#isInterceptAuto--) | Microsoft Workbook'un trend çizgisinin kesişimini otomatik olarak belirleyip belirlemediğini gösterir. |
| [isNameAuto()](#isNameAuto--) | Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür. |
| [isVisible()](#isVisible--) | Çizginin görünür olup olmadığını temsil eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir. |
| [setBackward(double value)](#setBackward-double-) | Trend çizgisinin geriye doğru uzandığı dönem (veya dağılım grafiğindeki birimler) sayısını döndürür veya ayarlar. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Bir çizginin başlangıcı için ok başının uzunluğunu belirtir. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Bir çizginin başlangıcı için ok başının genişliğini belirtir. |
| [setBeginType(int value)](#setBeginType-int-) | Bir çizginin başlangıcı için bir ok başı belirtir. |
| [setCapType(int value)](#setCapType-int-) | Bitiş kapaklarını belirtir. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Satırın [Color](../../com.aspose.cells/color) değerini temsil eder. |
| [setCompoundType(int value)](#setCompoundType-int-) | Bileşik çizgi tipini belirtir |
| [setDashType(int value)](#setDashType-int-) | Kesikli çizgi tipini belirtir |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Trend çizgisinin denkleminin grafikte (R-kare değeriyle aynı veri etiketinde) gösterilip gösterilmediğini temsil eder. |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Trend çizgisinin R-kare değerinin grafikte (denklemin aynı veri etiketinde) gösterilip gösterilmediğini temsil eder. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Bir çizginin ucundaki ok başının uzunluğunu belirtir. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Bir çizginin ucundaki ok başının genişliğini belirtir. |
| [setEndType(int value)](#setEndType-int-) | Bir çizginin ucunda bir ok başı belirtir. |
| [setFormattingType(int value)](#setFormattingType-int-) | Biçim türünü ayarlar. |
| [setForward(double value)](#setForward-double-) | Trend çizgisinin ileri doğru uzandığı dönem (veya dağılım grafiğindeki birim) sayısını alır veya ayarlar. |
| [setIntercept(double value)](#setIntercept-double-) | Trend çizgisinin değer eksenini kestiği noktayı alır veya ayarlar. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Microsoft Workbook'un trend çizgisinin kesişimini otomatik olarak belirleyip belirlemediğini ayarlar. |
| [setJoinType(int value)](#setJoinType-int-) | Birleştirme kapaklarını belirtir. |
| [setName(String value)](#setName-java.lang.String-) | Trend çizgisinin adını döndürür. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür. |
| [setOrder(int value)](#setOrder-int-) | Trend çizgisi tipi Polinom olduğunda trend çizgisi derecesini (1'den büyük bir tam sayı) alır veya ayarlar. |
| [setPeriod(int value)](#setPeriod-int-) | Hareketli ortalama trend çizgisi için periyodu alır veya ayarlar. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Trend çizgisinin geriye doğru uzadığı dönem (veya dağılım grafiğindeki birim) sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır. Grafik tipi sütun ise, dönem sayısı 0 ile 0.5 arasında olmalıdır.

**Returns:**
double
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
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Belirtilen seriye ait DataLabels nesnesini temsil eder.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Trend çizgisinin denkleminin grafikte (R-kare değeriyle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Trend çizgisinin R-kare değerinin grafikte (denklemle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar.

**Returns:**
boolean
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
### getForward() {#getForward--}
```
public double getForward()
```


Trend çizgisinin ileri doğru uzadığı dönem (veya dağılım grafiğindeki birim) sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Gradyan doldurmayı temsil eder.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Trend çizgisinin değer eksenini kestiği noktayı alır veya ayarlar.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Birleştirme kapaklarını belirtir.

Bakınız [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Bu trend çizgisine göre gösterge girişini alır.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Trend çizgisinin adını döndürür.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Trend çizgi türü Polinom olduğunda trend çizgi derecesini (1'den büyük bir tam sayı) döndürür veya ayarlar. Derece 2 ile 6 arasında olmalıdır.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Hareketli ortalama trend çizgisi için periyodu alır veya ayarlar.

**Remarks**

Bu değer 2 ile 255 arasında olmalıdır. Ve serideki grafik noktalarının sayısından daha az olmalıdır.

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
### getType() {#getType--}
```
public int getType()
```


Trend çizgisi tipini döndürür.

Bakın [TrendlineType](../../com.aspose.cells/trendlinetype).

**Returns:**
int
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
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Microsoft Workbook'un trend çizgisinin kesişimini otomatik olarak belirleyip belirlemediğini gösterir.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür.

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

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Trend çizgisinin geriye doğru uzadığı dönem (veya dağılım grafiğindeki birim) sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır. Grafik tipi sütun ise, dönem sayısı 0 ile 0.5 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Trend çizgisinin denkleminin grafikte (R-kare değeriyle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Trend çizgisinin R-kare değerinin grafikte (denklemle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Trend çizgisinin ileri doğru uzadığı dönem (veya dağılım grafiğindeki birim) sayısını döndürür veya ayarlar. Dönem sayısı sıfırdan büyük veya eşit olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Trend çizgisinin değer eksenini kestiği noktayı alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Microsoft Workbook'un trend çizgisinin kesişimini otomatik olarak belirleyip belirlemediğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Trend çizgisinin adını döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Trend çizgi türü Polinom olduğunda trend çizgi derecesini (1'den büyük bir tam sayı) döndürür veya ayarlar. Derece 2 ile 6 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Hareketli ortalama trend çizgisi için periyodu alır veya ayarlar.

**Remarks**

Bu değer 2 ile 255 arasında olmalıdır. Ve serideki grafik noktalarının sayısından daha az olmalıdır.

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

