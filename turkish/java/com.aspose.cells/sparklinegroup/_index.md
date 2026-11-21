---
title: "SparklineGroup"
second_title: "Aspose.Cells for Java API Referansı"
description: "bir sparkline grubuna düzenlenir."
type: docs
url: /tr/java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         // Create CellsColor
         CellsColor clr = book.createCellsColor();
         clr.setColor(Color.getOrange());
         group.setSeriesColor(clr);
 
         // set the high points are colored green and the low points are colored red
         group.setShowHighPoint(true);
         group.setShowLowPoint(true);
         group.getHighPointColor().setColor(Color.getGreen());
         group.getLowPointColor().setColor(Color.getRed());
         // set line weight 
         group.setLineWeight(1.0);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir. |
| [getFirstPointColor()](#getFirstPointColor--) | Sparkline grubundaki ilk veri noktasının rengini alır. |
| [getHighPointColor()](#getHighPointColor--) | Sparkline grubundaki en yüksek veri noktalarının rengini alır. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Sparkline grubundaki yatay eksenin rengini alır. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Sparkline verileri için tarih değerlerini içeren aralığı temsil eder. |
| [getLastPointColor()](#getLastPointColor--) | Sparkline grubundaki son veri noktasının rengini alır. |
| [getLineWeight()](#getLineWeight--) | Sparkline grubundaki her satır sparkline için çizgi kalınlığını, puan biriminde alır. |
| [getLowPointColor()](#getLowPointColor--) | Sparkline grubundaki en düşük veri noktalarının rengini alır. |
| [getMarkersColor()](#getMarkersColor--) | Sparkline grubundaki her satır sparkline'deki noktaların rengini alır. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Sparkline grubundaki negatif değerlerin rengini alır. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Boş hücrelerin nasıl çizileceğini gösterir. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Çizim verisinin sağdan sola olup olmadığını gösterir. |
| [getPresetStyle()](#getPresetStyle--) | Sparkline grubunun önceden ayarlanmış stil tipini alır. |
| [getSeriesColor()](#getSeriesColor--) | Sparkline grubundaki sparklineların rengini alır. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Sparkline grubundaki ilk veri noktasının vurgulanıp vurgulanmayacağını gösterir. |
| [getShowHighPoint()](#getShowHighPoint--) | Sparkline grubundaki verilerin en yüksek noktalarını vurgulayıp vurgulanmayacağını gösterir. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Sparkline yatay ekseninin gösterilip gösterilmeyeceğini gösterir. |
| [getShowLastPoint()](#getShowLastPoint--) | Sparkline grubundaki verinin son noktasını vurgulayıp vurgulanmayacağını gösterir. |
| [getShowLowPoint()](#getShowLowPoint--) | Sparkline grubundaki verilerin en düşük noktalarını vurgulayıp vurgulanmayacağını gösterir. |
| [getShowMarkers()](#getShowMarkers--) | Sparkline grubundaki her satır sparkline'ındaki her noktayı vurgulayıp vurgulanmayacağını gösterir. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçiyle vurgulayıp vurgulanmayacağını gösterir. |
| [getSparklineCollection()](#getSparklineCollection--) | [Sparkline](../../com.aspose.cells/sparkline) nesnesinin koleksiyonunu alır. |
| [getSparklines()](#getSparklines--) | [Sparkline](../../com.aspose.cells/sparkline) nesnesinin koleksiyonunu alır. |
| [getType()](#getType--) | Sparkline grubunun sparkline tipini gösterir. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Dikey eksen için özel maksimum değeri alır. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Dikey eksen maksimum değer tipini temsil eder. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Dikey eksen için özel minimum değeri alır. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Dikey eksen minimum değer tipini temsil eder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Sparkline grubunun veri aralığını ve konum aralığını sıfırlar. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki verinin ilk noktasının rengini ayarlar. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki verilerin en yüksek noktalarının rengini ayarlar. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki yatay eksenin rengini ayarlar. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Sparkline verileri için tarih değerlerini içeren aralığı temsil eder. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki verinin son noktasının rengini ayarlar. |
| [setLineWeight(double value)](#setLineWeight-double-) | Sparkline grubundaki her satır sparkline'ındaki çizgi kalınlığını, puan biriminde ayarlar. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki verilerin en düşük noktalarının rengini ayarlar. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki her satır sparkline'ındaki noktaların rengini ayarlar. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki negatif değerlerin rengini ayarlar. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Boş hücrelerin nasıl çizileceğini gösterir. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Çizim verisinin sağdan sola olup olmadığını gösterir. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Sparkline grubunun önceden ayarlanmış stil tipini ayarlar. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Sparkline grubundaki sparkline'ların rengini ayarlar. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Sparkline grubundaki ilk veri noktasının vurgulanıp vurgulanmayacağını gösterir. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Sparkline grubundaki verilerin en yüksek noktalarını vurgulayıp vurgulanmayacağını gösterir. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Sparkline yatay ekseninin gösterilip gösterilmeyeceğini gösterir. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Sparkline grubundaki verinin son noktasını vurgulayıp vurgulanmayacağını gösterir. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Sparkline grubundaki verilerin en düşük noktalarını vurgulayıp vurgulanmayacağını gösterir. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Sparkline grubundaki her satır sparkline'ındaki her noktayı vurgulayıp vurgulanmayacağını gösterir. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçiyle vurgulayıp vurgulanmayacağını gösterir. |
| [setType(int value)](#setType-int-) | Sparkline grubunun sparkline tipini gösterir. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Dikey eksen için özel maksimum değeri ayarlar. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Belirtilen eksen değer tipiyle sparkline dikey ekseni için özel maksimum değeri ayarlar. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Dikey eksen maksimum değer tipini temsil eder. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Dikey eksen için özel minimum değeri ayarlar. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Belirtilen eksen değer türüyle birlikte sparkline dikey ekseni için özel minimum değeri ayarlar. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Dikey eksen minimum değer tipini temsil eder. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayHidden() {#getDisplayHidden--}
```
public boolean getDisplayHidden()
```


Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Sparkline grubundaki ilk veri noktasının rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Sparkline grubundaki en yüksek veri noktalarının rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Sparkline grubundaki yatay eksenin rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Sparkline verileri için tarih değerlerini içeren aralığı temsil eder.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Sparkline grubundaki son veri noktasının rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Sparkline grubundaki her satır sparkline için çizgi kalınlığını, puan biriminde alır.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Sparkline grubundaki en düşük veri noktalarının rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Sparkline grubundaki her satır sparkline'deki noktaların rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Sparkline grubundaki negatif değerlerin rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Boş hücrelerin nasıl çizileceğini gösterir.

Bakınız [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Çizim verisinin sağdan sola olup olmadığını gösterir.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Sparkline grubunun önceden ayarlanmış stil tipini alır.

Bakınız [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Bu özellik ayarlanırsa, şu özellikler: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor kapsanacaktır. Bu yüzden önce özelliği ayarlayın, ardından diğerlerini ayarlayın.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Sparkline grubundaki sparklineların rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Sparkline grubundaki ilk veri noktasının vurgulanıp vurgulanmayacağını gösterir.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Sparkline grubundaki verilerin en yüksek noktalarını vurgulayıp vurgulanmayacağını gösterir.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Sparkline yatay ekseninin gösterilip gösterilmeyeceğini belirtir. Yatay eksen, sparkline sıfır eksenini geçen verilere sahipse görünür.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Sparkline grubundaki verinin son noktasını vurgulayıp vurgulanmayacağını gösterir.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Sparkline grubundaki verilerin en düşük noktalarını vurgulayıp vurgulanmayacağını gösterir.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Sparkline grubundaki her satır sparkline'ındaki her noktayı vurgulayıp vurgulanmayacağını gösterir.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçiyle vurgulayıp vurgulanmayacağını gösterir.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


[Sparkline](../../com.aspose.cells/sparkline) nesnesinin koleksiyonunu alır.

**Remarks**

NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen SparklineGroup.Sparklines özelliğini kullanın. Bu özellik Kasım 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


[Sparkline](../../com.aspose.cells/sparkline) nesnesinin koleksiyonunu alır.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Sparkline grubunun sparkline tipini gösterir.

Bakınız [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Dikey eksen için özel maksimum değeri alır.

**Remarks**

Bu özellik ayarlanırsa, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) olacaktır.

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Dikey eksen maksimum değer tipini temsil eder.

Bakınız [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Dikey eksen için özel minimum değeri alır.

**Remarks**

Bu özellik ayarlanırsa, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) olacaktır.

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Dikey eksen minimum değer tipini temsil eder.

Bakınız [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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




### resetRanges(String dataRange, boolean isVertical, CellArea locationRange) {#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public void resetRanges(String dataRange, boolean isVertical, CellArea locationRange)
```


Sparkline grubunun veri aralığını ve konum aralığını sıfırlar. Bu yöntem, gruptaki orijinal sparkline öğelerini temizleyecek ve yeni aralıklar için yeni sparkline öğeleri oluşturacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataRange | java.lang.String | Sparkline grubunun yeni veri aralığını belirtir. |
| isVertical | boolean | Sparklineları yeni veri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Sparklineların yerleştirileceği konumu belirtir. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Sparkline grubundaki verinin ilk noktasının rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Sparkline grubundaki verilerin en yüksek noktalarının rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Sparkline grubundaki yatay eksenin rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Sparkline verileri için tarih değerlerini içeren aralığı temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Sparkline grubundaki verinin son noktasının rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Sparkline grubundaki her satır sparkline'ındaki çizgi kalınlığını, puan biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Sparkline grubundaki verilerin en düşük noktalarının rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Sparkline grubundaki her satır sparkline'ındaki noktaların rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Sparkline grubundaki negatif değerlerin rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Boş hücrelerin nasıl çizileceğini gösterir.

Bakınız [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Çizim verisinin sağdan sola olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Sparkline grubunun önceden ayarlanmış stil tipini ayarlar.

Bakınız [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Bu özellik ayarlanırsa, şu özellikler: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor kapsanacaktır. Bu yüzden önce özelliği ayarlayın, ardından diğerlerini ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Sparkline grubundaki sparkline'ların rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Sparkline grubundaki ilk veri noktasının vurgulanıp vurgulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Sparkline grubundaki verilerin en yüksek noktalarını vurgulayıp vurgulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Sparkline yatay ekseninin gösterilip gösterilmeyeceğini belirtir. Yatay eksen, sparkline sıfır eksenini geçen verilere sahipse görünür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Sparkline grubundaki verinin son noktasını vurgulayıp vurgulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Sparkline grubundaki verilerin en düşük noktalarını vurgulayıp vurgulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Sparkline grubundaki her satır sparkline'ındaki her noktayı vurgulayıp vurgulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçiyle vurgulayıp vurgulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Sparkline grubunun sparkline tipini gösterir.

Bakınız [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Dikey eksen için özel maksimum değeri ayarlar.

**Remarks**

Bu özellik ayarlanırsa, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Belirtilen eksen değer tipiyle sparkline dikey ekseni için özel maksimum değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Eksen maksimum değerinin nasıl uygulandığını belirten tür. |
| value | double | Dikey eksenin özel maksimum değeri. Tür [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) değilse göz ardı edilir. |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Dikey eksen maksimum değer tipini temsil eder.

Bakınız [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Dikey eksen için özel minimum değeri ayarlar.

**Remarks**

Bu özellik ayarlanırsa, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Belirtilen eksen değer türüyle birlikte sparkline dikey ekseni için özel minimum değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Eksen minimum değerinin nasıl uygulandığını belirten tür. |
| value | double | Dikey eksenin özel minimum değeri. Tür [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM) değilse göz ardı edilir. |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Dikey eksen minimum değer tipini temsil eder.

Bakınız [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

