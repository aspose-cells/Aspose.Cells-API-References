---
title: "Axis"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir grafiğin eksenini temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Bir grafiğin eksenini temsil eden nesneyi kapsüller.

**Example**

Aşağıdaki kodlardan, Axis'in birim, maksimum ve minimum değerlerini nasıl ayarlayacağınızı öğrenebilirsiniz.

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | [getArea()](../../com.aspose.cells/axis\#getArea--) metodunu alır. |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Değer ekseninin kategori eksenini kategoriler arasında kesip kesmediğini temsil eder. |
| [getAxisLabels()](#getAxisLabels--) | Chart.Calculate() metodunu çağırdıktan sonra eksenin etiketlerini alır. |
| [getAxisLine()](#getAxisLine--) | Bir Axis'in görünümünü alır. |
| [getAxisTexts()](#getAxisTexts--) | Chart.Calculate() metodunu çağırdıktan sonra eksenin etiketlerini alır. |
| [getBaseUnitScale()](#getBaseUnitScale--) | Kategori ekseni için temel birim ölçeğini temsil eder. |
| [getBins()](#getBins--) | Bir grafik (Histogram/Pareto) eksenindeki kutucukları temsil eder |
| [getCategoryType()](#getCategoryType--) | Kategori ekseninin tipini temsil eder. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Değer ekseninde, kategori ekseninin onu kestiği noktayı temsil eder. |
| [getCrossType()](#getCrossType--) | Belirtilen eksende diğer eksenin kesildiği yerdeki [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) metodunu temsil eder. |
| [getCustUnit()](#getCustUnit--) | Görüntü birimi için özel bir değer belirtir. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Görüntü birimi için özel bir değer belirtir. |
| [getCustomUnit()](#getCustomUnit--) | Görüntü birimi için özel bir değer belirtir. |
| [getDisplayUnit()](#getDisplayUnit--) | Belirtilen eksen için birim etiketini temsil eder. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Belirtilen grafikte bir eksende birim etiketini temsil eder. |
| [getLogBase()](#getLogBase--) | Logaritmik tabanı temsil eder. |
| [getMajorGridLines()](#getMajorGridLines--) | Bir grafik eksenindeki ana ızgara çizgilerini temsil eder. |
| [getMajorTickMark()](#getMajorTickMark--) | Belirtilen eksen için ana işaret çubuğunun türünü temsil eder. |
| [getMajorUnit()](#getMajorUnit--) | Eksen için ana birimleri temsil eder. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [getMaxValue()](#getMaxValue--) | Değer eksenindeki maksimum değeri temsil eder. |
| [getMinValue()](#getMinValue--) | Değer eksenindeki minimum değeri temsil eder. |
| [getMinorGridLines()](#getMinorGridLines--) | Bir grafik eksenindeki alt ızgara çizgilerini temsil eder. |
| [getMinorTickMark()](#getMinorTickMark--) | Belirtilen eksen için alt işaret çubuğunun türünü temsil eder. |
| [getMinorUnit()](#getMinorUnit--) | Eksen için alt birimleri temsil eder. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Belirtilen eksen üzerindeki işaret çubuğu etiketlerinin konumunu temsil eder. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | İşaret çubuğu etiketleri arasındaki kategori veya seri sayısını temsil eder. |
| [getTickLabels()](#getTickLabels--) | Belirtilen eksen için işaret çubuğu etiketlerini temsil eden bir [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) nesnesi döndürür. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | İşaret çubukları arasındaki kategori veya seri sayısını döndürür veya ayarlar. |
| [getTitle()](#getTitle--) | Bu eksenin grafikteki başlığını alır. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Etiketlerin çok seviyeli gösterilip gösterilmeyeceğini belirtir. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | İşaret çubuğu etiketlerinin aralığının otomatik olup olmadığını belirtir. |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Eksenin ana biriminin otomatik olarak atanıp atanmadığını belirtir. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Maksimum değerin otomatik olarak atanıp atanmadığını belirtir. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Minimum değerin otomatik olarak atanıp atanmadığını belirtir. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Eksenin alt biriminin otomatik olarak atanıp atanmadığını belirtir. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Temel birimin otomatik olup olmadığını temsil eder. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Belirtilen eksende görüntü birimi etiketinin gösterilip gösterilmediğini temsil eder. |
| [isLogarithmic()](#isLogarithmic--) | Değer ekseni ölçek tipinin logaritmik olup olmadığını temsil eder. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Microsoft Excel'in veri noktalarını sondan başa doğru çizip çizmediğini temsil eder. |
| [isVisible()](#isVisible--) | Eksenin görünür olup olmadığını temsil eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | İşaret çubuğu etiketlerinin aralığının otomatik olup olmadığını belirtir. |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Eksenin ana biriminin otomatik olarak atanıp atanmadığını belirtir. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Maksimum değerin otomatik olarak atanıp atanmadığını belirtir. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Minimum değerin otomatik olarak atanıp atanmadığını belirtir. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Eksenin alt biriminin otomatik olarak atanıp atanmadığını belirtir. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Değer ekseninin kategori eksenini kategoriler arasında kesip kesmediğini temsil eder. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Temel birimin otomatik olup olmadığını temsil eder. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Kategori ekseni için temel birim ölçeğini temsil eder. |
| [setCategoryType(int value)](#setCategoryType-int-) | Kategori ekseninin tipini temsil eder. |
| [setCrossAt(double value)](#setCrossAt-double-) | Değer ekseninde, kategori ekseninin onu kestiği noktayı temsil eder. |
| [setCrossType(int value)](#setCrossType-int-) | Belirtilen eksende diğer eksenin kesildiği yerdeki [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) metodunu temsil eder. |
| [setCustUnit(int value)](#setCustUnit-int-) | Görüntü birimi için özel bir değer belirtir. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Görüntü birimi için özel bir değer belirtir. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Görüntü birimi için özel bir değer belirtir. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Belirtilen eksen için birim etiketini temsil eder. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Belirtilen eksende görüntü birimi etiketinin gösterilip gösterilmediğini temsil eder. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Etiketlerin çok seviyeli gösterilip gösterilmeyeceğini belirtir. |
| [setLogBase(double value)](#setLogBase-double-) | Logaritmik tabanı temsil eder. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Değer ekseni ölçek tipinin logaritmik olup olmadığını temsil eder. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Belirtilen eksen için ana işaret çubuğunun türünü temsil eder. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Eksen için ana birimleri temsil eder. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Değer eksenindeki maksimum değeri temsil eder. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Değer eksenindeki minimum değeri temsil eder. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Belirtilen eksen için alt işaret çubuğunun türünü temsil eder. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Eksen için alt birimleri temsil eder. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Microsoft Excel'in veri noktalarını sondan başa doğru çizip çizmediğini temsil eder. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Belirtilen eksen üzerindeki işaret çubuğu etiketlerinin konumunu temsil eder. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | İşaret çubuğu etiketleri arasındaki kategori veya seri sayısını temsil eder. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | İşaret çubukları arasındaki kategori veya seri sayısını döndürür veya ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Eksenin görünür olup olmadığını temsil eder. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


[getArea()](../../com.aspose.cells/axis\#getArea--) metodunu alır.

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Değer ekseninin kategori eksenini kategoriler arasında kesip kesmediğini temsil eder.

**Remarks**

Bu özellik yalnızca kategori eksenlerine uygulanır ve 3D grafiklere uygulanmaz.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Chart.Calculate() metodunu çağırdıktan sonra eksenin etiketlerini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Axis.GetAxisTexts yöntemini kullanın. Bu özellik Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Bir Axis'in görünümünü alır.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Chart.Calculate() metodunu çağırdıktan sonra eksenin etiketlerini alır.

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Kategori ekseni için temel birim ölçeğini temsil eder.

Bak [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Yalnızca CategoryType özelliği TimeScale olarak ayarlandığında etkili olur.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Bir grafik (Histogram/Pareto) eksenindeki kutucukları temsil eder

**Remarks**

Yalnızca Histogram veya Pareto grafiği için.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Kategori ekseninin tipini temsil eder.

Bak [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


Değer ekseninde, kategori ekseninin onu kestiği noktayı temsil eder.

**Remarks**

Sayı, kategori eksenine uygulandığında tam sayı olmalıdır. Ve değer 1 ile 31999 arasında olmalıdır.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Belirtilen eksende diğer eksenin kesildiği yerdeki [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) metodunu temsil eder.

Bak [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Görüntü birimi için özel bir değer belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Axis.CustomUnit özelliğini kullanın. Bu özellik Ocak 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Görüntü birimi için özel bir değer belirtir.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Görüntü birimi için özel bir değer belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Axis.CustomDisplayUnit özelliğini kullanın. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Belirtilen eksen için birim etiketini temsil eder.

Bak [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Belirtilen grafikte bir eksende bir birim etiketi temsil eder. Birim etiketleri büyük değerleri (örneğin milyonlar ya da milyarlar) grafiklemek için faydalıdır.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Logaritmik tabanı temsil eder. Varsayılan değer 10'dur.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Bir grafik eksenindeki ana ızgara çizgilerini temsil eder.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


Belirtilen eksen için ana işaret çubuğunun türünü temsil eder.

Bak [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Eksen için ana birimleri temsil eder.

**Remarks**

Ana birimler sıfırdan büyük olmalıdır.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Kategori ekseni için ana birim ölçeğini temsil eder.

Bak [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Değer eksenindeki maksimum değeri temsil eder.

**Remarks**

maxValue türü yalnızca double veya DateTime olabilir.

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Değer eksenindeki minimum değeri temsil eder.

**Remarks**

minValue türü yalnızca double veya DateTime olabilir.

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Bir grafik eksenindeki alt ızgara çizgilerini temsil eder.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Belirtilen eksen için alt işaret çubuğunun türünü temsil eder.

Bak [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Eksen için alt birimleri temsil eder.

**Remarks**

Küçük birimler sıfırdan büyük olmalıdır.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Kategori ekseni için ana birim ölçeğini temsil eder.

Bak [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


Belirtilen eksen üzerindeki işaret çubuğu etiketlerinin konumunu temsil eder.

Bak [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Tik işareti etiketleri arasındaki kategori veya seri sayısını temsil eder. Yalnızca kategori ve seri eksenlerine uygulanır.

**Remarks**

Sayı 1 ile 31999 arasında olmalıdır.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Belirtilen eksen için işaret çubuğu etiketlerini temsil eden bir [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) nesnesi döndürür.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Tik işaretleri arasındaki kategori veya seri sayısını döndürür veya ayarlar. Yalnızca kategori ve seri eksenlerine uygulanır.

**Remarks**

Sayı 1 ile 31999 arasında olmalıdır.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Bu eksenin grafikteki başlığını alır.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Etiketlerin çok seviyeli gösterilip gösterilmeyeceğini belirtir.

**Remarks**

Yalnızca kategori ekseni için geçerlidir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


İşaret çubuğu etiketlerinin aralığının otomatik olup olmadığını belirtir.

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Eksenin ana biriminin otomatik olarak atanıp atanmadığını belirtir.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Maksimum değerin otomatik olarak atanıp atanmadığını belirtir.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Minimum değerin otomatik olarak atanıp atanmadığını belirtir.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Eksenin alt biriminin otomatik olarak atanıp atanmadığını belirtir.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Temel birimin otomatik olup olmadığını temsil eder.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Belirtilen eksende görüntü birimi etiketinin gösterilip gösterilmediğini temsil eder.

**Remarks**

Varsayılan değer True'dur. Yalnızca [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE) olmadığında çalışır.

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Değer ekseni ölçek tipinin logaritmik olup olmadığını temsil eder.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Microsoft Excel'in veri noktalarını sondan başa doğru çizip çizmediğini temsil eder.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Eksenin görünür olup olmadığını temsil eder.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


İşaret çubuğu etiketlerinin aralığının otomatik olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Eksenin ana biriminin otomatik olarak atanıp atanmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Maksimum değerin otomatik olarak atanıp atanmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Minimum değerin otomatik olarak atanıp atanmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Eksenin alt biriminin otomatik olarak atanıp atanmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Değer ekseninin kategori eksenini kategoriler arasında kesip kesmediğini temsil eder.

**Remarks**

Bu özellik yalnızca kategori eksenlerine uygulanır ve 3D grafiklere uygulanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Temel birimin otomatik olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Kategori ekseni için temel birim ölçeğini temsil eder.

Bak [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Yalnızca CategoryType özelliği TimeScale olarak ayarlandığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Kategori ekseninin tipini temsil eder.

Bak [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Değer ekseninde, kategori ekseninin onu kestiği noktayı temsil eder.

**Remarks**

Sayı, kategori eksenine uygulandığında tam sayı olmalıdır. Ve değer 1 ile 31999 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Belirtilen eksende diğer eksenin kesildiği yerdeki [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) metodunu temsil eder.

Bak [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Görüntü birimi için özel bir değer belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Axis.CustomUnit özelliğini kullanın. Bu özellik Ocak 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Görüntü birimi için özel bir değer belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Görüntü birimi için özel bir değer belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Axis.CustomDisplayUnit özelliğini kullanın. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Belirtilen eksen için birim etiketini temsil eder.

Bak [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Belirtilen eksende görüntü birimi etiketinin gösterilip gösterilmediğini temsil eder.

**Remarks**

Varsayılan değer True'dur. Yalnızca [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE) olmadığında çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Etiketlerin çok seviyeli gösterilip gösterilmeyeceğini belirtir.

**Remarks**

Yalnızca kategori ekseni için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Logaritmik tabanı temsil eder. Varsayılan değer 10'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Değer ekseni ölçek tipinin logaritmik olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Belirtilen eksen için ana işaret çubuğunun türünü temsil eder.

Bak [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Eksen için ana birimleri temsil eder.

**Remarks**

Ana birimler sıfırdan büyük olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Kategori ekseni için ana birim ölçeğini temsil eder.

Bak [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Değer eksenindeki maksimum değeri temsil eder.

**Remarks**

maxValue türü yalnızca double veya DateTime olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Değer eksenindeki minimum değeri temsil eder.

**Remarks**

minValue türü yalnızca double veya DateTime olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Belirtilen eksen için alt işaret çubuğunun türünü temsil eder.

Bak [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Eksen için alt birimleri temsil eder.

**Remarks**

Küçük birimler sıfırdan büyük olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Kategori ekseni için ana birim ölçeğini temsil eder.

Bak [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Microsoft Excel'in veri noktalarını sondan başa doğru çizip çizmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Belirtilen eksen üzerindeki işaret çubuğu etiketlerinin konumunu temsil eder.

Bak [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Tik işareti etiketleri arasındaki kategori veya seri sayısını temsil eder. Yalnızca kategori ve seri eksenlerine uygulanır.

**Remarks**

Sayı 1 ile 31999 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Tik işaretleri arasındaki kategori veya seri sayısını döndürür veya ayarlar. Yalnızca kategori ve seri eksenlerine uygulanır.

**Remarks**

Sayı 1 ile 31999 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Eksenin görünür olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

