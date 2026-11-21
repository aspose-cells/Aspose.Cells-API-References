---
title: "Grafik"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tek bir Excel grafiğini temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Tek bir Excel grafiğini temsil eden nesneyi kapsar.

**Example**

Aşağıdaki kodlar .NET kodlarıyla bir grafik oluşturmayı gösterir.

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
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [calculate()](#calculate--) | Konumları otomatik atanmışsa, çizim alanı ve eksenlerin özel konumlarını hesaplar. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Konumları otomatik atanmışsa, Çizim Alanı ve eksenlerin özel konumunu, Grafik Hesaplama Seçenekleri ile hesaplar. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Önceden ayarlanmış bir şablonla grafik tipini değiştir. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Grafiğin gerçek boyutunu piksel biriminde alır. |
| [getActualSize()](#getActualSize--) | Grafiğin gerçek boyutunu piksel biriminde alır. |
| [getAutoScaling()](#getAutoScaling--) | Microsoft Excel, 3B grafiği eşdeğer 2B grafiğe daha yakın bir boyuta ölçeklendiriyorsa doğru (true) döner. |
| [getBackWall()](#getBackWall--) | 3B grafiğin arka duvarını temsil eden bir [getWalls()](../../com.aspose.cells/chart\#getWalls--) nesnesi döndürür. |
| [getCategoryAxis()](#getCategoryAxis--) | Grafiğin X eksenini alır. |
| [getChartArea()](#getChartArea--) | Çalışma sayfasındaki grafik alanını alır. |
| [getChartDataRange()](#getChartDataRange--) | Grafiğin veri kaynağı aralığını alır. |
| [getChartDataTable()](#getChartDataTable--) | Grafik veri tablosunu temsil eder. |
| [getChartObject()](#getChartObject--) | chartShape'ı temsil eder; |
| [getChartShape()](#getChartShape--) | chartShape'ı temsil eder; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | 3-D grafiğin derinliğini, grafik genişliğinin yüzde olarak (20 ile 2000 yüzde arasında) temsil eder. |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | \#N/A değerinin boş olarak gösterilip gösterilmeyeceğini belirtir. |
| [getElevation()](#getElevation--) | 3-D grafik görünümünün yüksekliğini derece cinsinden temsil eder. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Grafikte filtrelenen veri serilerini temsil eden bir [SeriesCollection](../../com.aspose.cells/seriescollection) koleksiyonunu alır. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) alır. |
| [getFloor()](#getFloor--) | 3-D grafiğin duvarlarını temsil eden bir [getFloor()](../../com.aspose.cells/chart\#getFloor--) nesnesi döndürür. |
| [getGapDepth()](#getGapDepth--) | 3-D grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzde olarak alır. |
| [getGapWidth()](#getGapWidth--) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzde olarak döndürür veya ayarlar. |
| [getHeightPercent()](#getHeightPercent--) | 3-D grafiğin yüksekliğini, grafik genişliğinin yüzde olarak (5 ile 500 yüzde arasında) döndürür veya ayarlar. |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Grafik PivotChart olduğunda sadece pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini belirtir. |
| [getIs3D()](#getIs3D--) | Grafiğin 3d grafik olup olmadığını belirtir. |
| [getLegend()](#getLegend--) | Grafik açıklamasını alır. |
| [getLine()](#getLine--) | Çizgiyi alır. |
| [getNSeries()](#getNSeries--) | Grafikteki veri serilerini temsil eden bir [SeriesCollection](../../com.aspose.cells/seriescollection) koleksiyonunu alır. |
| [getName()](#getName--) | Grafiğin adını alır. |
| [getPageSetup()](#getPageSetup--) | Bu grafikte sayfa ayarı açıklamasını temsil eder. |
| [getPerspective()](#getPerspective--) | three\\u9225\\u6178 boyutlu grafik görünümü için perspektifi döndürür veya ayarlar. |
| [getPivotOptions()](#getPivotOptions--) | Grafikte görünen pivot kontrollerini belirtir |
| [getPivotSource()](#getPivotSource--) | Kaynak, pivot tablo verisidir. |
| [getPlacement()](#getPlacement--) | Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [getPlotArea()](#getPlotArea--) | Eksen işaret etiketi etiketlerini içeren grafiğin çizim alanını alır. |
| [getPlotBy()](#getPlotBy--) | Satır ya da sütun bazında çizimin olup olmadığını alır. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Boş hücrelerin nasıl çizileceğini alır. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir. |
| [getPrintSize()](#getPrintSize--) | Yazdırılan grafik boyutunu alır. |
| [getRightAngleAxes()](#getRightAngleAxes--) | Grafik eksenleri dik açı oluşturuyorsa doğru. |
| [getRotationAngle()](#getRotationAngle--) | 3B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Grafiğin ikinci X eksenini alır. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Grafiğin ikinci Y eksenini alır. |
| [getSeriesAxis()](#getSeriesAxis--) | Grafiğin seri eksenini alır. |
| [getShapes()](#getShapes--) | Bu grafikteki tüm çizim şekillerini döndürür. |
| [getShowDataTable()](#getShowDataTable--) | Grafiğin bir veri tablosu gösterip göstermediğini belirten bir değeri alır. |
| [getShowLegend()](#getShowLegend--) | Grafik açıklamasının gösterilip gösterilmeyeceğini belirten bir değeri alır. |
| [getSideWall()](#getSideWall--) | 3B grafiğin yan duvarını temsil eden bir [getWalls()](../../com.aspose.cells/chart\#getWalls--) nesnesini döndürür. |
| [getSizeWithWindow()](#getSizeWithWindow--) | Microsoft Excel grafiği, grafik sayfası penceresinin boyutuna uyacak şekilde yeniden boyutlandırıyorsa doğru. |
| [getStyle()](#getStyle--) | Yerleşik stili alır. |
| [getSubTitle()](#getSubTitle--) | Grafiğin alt başlığını alır. |
| [getTitle()](#getTitle--) | Grafiğin başlığını alır. |
| [getType()](#getType--) | Bir grafiğin tipini alır. |
| [getValueAxis()](#getValueAxis--) | Grafiğin Y eksenini alır. |
| [getWalls()](#getWalls--) | 3B grafiğin duvarlarını temsil eden bir [getWalls()](../../com.aspose.cells/chart\#getWalls--) nesnesini döndürür. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | Izgara çizgileri 3B grafikte iki boyutlu olarak çiziliyorsa doğru. |
| [getWorksheet()](#getWorksheet--) | Bu grafiği içeren çalışma sayfasını alır. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Grafikte hangi eksenlerin mevcut olduğunu döndürür. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Grafik tarafından referans verilen hücrenin olup olmadığını döndürür. |
| [isChartDataChanged()](#isChartDataChanged--) | Bir grafiğin veri kaynağının değişip değişmediğini algılar. |
| [isRectangularCornered()](#isRectangularCornered--) | Grafik alanının dikdörtgen köşeli olup olmadığını gösteren bir değer alır. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Hücrenin grafik tarafından referans alınıp alınmadığını döndürür. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Grafiği belirtilen konuma taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Grafiğin verilerini özet tablo (pivot table) üzerinden yeniler. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | Microsoft Excel, 3B grafiği eşdeğer 2B grafiğe daha yakın bir boyuta ölçeklendiriyorsa doğru (true) döner. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Grafik için veri aralığını belirtir. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | 3-D grafiğin derinliğini, grafik genişliğinin yüzde olarak (20 ile 2000 yüzde arasında) temsil eder. |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | \#N/A değerinin boş olarak gösterilip gösterilmeyeceğini belirtir. |
| [setElevation(int value)](#setElevation-int-) | 3-D grafik görünümünün yüksekliğini derece cinsinden temsil eder. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden ayarlar (dikeyden saat yönünde). |
| [setGapDepth(int value)](#setGapDepth-int-) | 3B grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzdesi olarak ayarlar. |
| [setGapWidth(int value)](#setGapWidth-int-) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzde olarak döndürür veya ayarlar. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | 3-D grafiğin yüksekliğini, grafik genişliğinin yüzde olarak (5 ile 500 yüzde arasında) döndürür veya ayarlar. |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Grafik PivotChart olduğunda sadece pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini belirtir. |
| [setName(String value)](#setName-java.lang.String-) | Grafiğin adını ayarlar. |
| [setPerspective(short value)](#setPerspective-short-) | three\\u9225\\u6178 boyutlu grafik görünümü için perspektifi döndürür veya ayarlar. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | Kaynak, pivot tablo verisidir. |
| [setPlacement(int value)](#setPlacement-int-) | Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Boş hücrelerin nasıl çizileceğini ayarlar. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir. |
| [setPrintSize(int value)](#setPrintSize-int-) | Yazdırılan grafik boyutunu ayarlar. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Grafik alanının dikdörtgen köşeli olup olmadığını gösteren bir değeri ayarlar. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | Grafik eksenleri dik açı oluşturuyorsa doğru. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | 3B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Grafiğin veri tablosu gösterip göstermediğini belirten bir değeri ayarlar. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Grafik açıklamasının (legend) gösterilip gösterilmeyeceğini belirten bir değeri ayarlar. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | Microsoft Excel grafiği, grafik sayfası penceresinin boyutuna uyacak şekilde yeniden boyutlandırıyorsa doğru. |
| [setStyle(int value)](#setStyle-int-) | Yerleşik stili ayarlar. |
| [setType(int value)](#setType-int-) | Bir grafiğin tipini ayarlar. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | Izgara çizgileri 3B grafikte iki boyutlu olarak çiziliyorsa doğru. |
| [switchRowColumn()](#switchRowColumn--) | Satır/kolonu değiştirir. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Grafik görüntüsünü oluşturur ve belirtilen formatta bir dosyaya kaydeder. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Grafik görüntüsünü oluşturur ve JPEG formatında bir dosyaya kaydeder. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Grafik PDF'ini oluşturur ve bir akışa kaydeder. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Grafik PDF'ini oluşturur ve bir akışa kaydeder. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Grafiği bir PDF dosyasına kaydeder. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Grafiği bir PDF dosyasına kaydeder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Konumları otomatik atanmışsa, çizim alanı ve eksenlerin özel konumlarını hesaplar.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Konumları otomatik atanmışsa, Çizim Alanı ve eksenlerin özel konumunu, Grafik Hesaplama Seçenekleri ile hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Önceden ayarlanmış bir şablonla grafik tipini değiştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| veri | byte[] | Grafik şablonu dosyasının (.crtx) verileri. |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Grafiğin gerçek boyutunu piksel biriminde alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Chart.getActualSize() yöntemini kullanın. Bu özellik Temmuz 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int[] - Gerçek boyut bir dizi içinde (genişlik ve yükseklik). [0] genişlik; [1] yükseklik.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Grafiğin gerçek boyutunu piksel biriminde alır.

**Returns:**
int[] - Gerçek boyut bir dizi içinde (genişlik ve yükseklik). [0] genişlik; [1] yükseklik.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


Microsoft Excel bir 3-B boyutlu grafiği, eşdeğer 2-B grafiğe daha yakın bir boyuta ölçeklendiriyorsa doğru (True). RightAngleAxes özelliği True olmalıdır.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


3B grafiğin arka duvarını temsil eden bir [getWalls()](../../com.aspose.cells/chart\#getWalls--) nesnesi döndürür.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Grafiğin X eksenini alır.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Çalışma sayfasındaki grafik alanını alır.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Grafiğin veri kaynağı aralığını alır.

**Remarks**

Yalnızca aralığı destekler. Series.Values, Name ve XValues sürekli bir aralıkta ise, onları içeren bir aralık döndürülecektir.

**Returns:**
java.lang.String - Veri kaynağı.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Grafik veri tablosunu temsil eder.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


chartShape'ı temsil eder;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


chartShape'ı temsil eder;

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Aspose.Cells.Charts.Chart.ChartObject özelliğini kullanın. Bu özellik OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


3-D grafiğin derinliğini, grafik genişliğinin yüzde olarak (20 ile 2000 yüzde arasında) temsil eder.

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


\#N/A değerinin boş olarak gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


3-D grafik görünümünün yüksekliğini derece cinsinden temsil eder.

**Remarks**

Grafik yüksekliği, grafiği gördüğünüz yüksekliği derece cinsinden ifade eder. Çoğu grafik türü için varsayılan değer 15'tir. Bu özelliğin değeri -90 ile 90 arasında olmalıdır, 3-B çubuk grafikleri dışında; bu grafiklerde 0 ile 44 arasında olmalıdır.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Grafikte filtrelenen veri serilerini temsil eden bir [SeriesCollection](../../com.aspose.cells/seriescollection) koleksiyonunu alır.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) alır. Yalnızca pasta, 3-B pasta ve halka grafiklerine uygulanır, 0 ile 360 arasında.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


3-D grafiğin duvarlarını temsil eden bir [getFloor()](../../com.aspose.cells/chart\#getFloor--) nesnesi döndürür.

**Remarks**

Bu özellik 3-B pasta grafiklerine uygulanmaz.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


3-B bir grafikte veri serileri arasındaki mesafeyi işaretçi genişliğinin yüzdesi olarak alır. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Çubuk veya sütun kümeleri arasındaki boşluğu çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


3-D grafiğin yüksekliğini, grafik genişliğinin yüzde olarak (5 ile 500 yüzde arasında) döndürür veya ayarlar.

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Grafik PivotChart olduğunda sadece pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini belirtir.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Grafiğin 3d grafik olup olmadığını belirtir.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Grafik açıklamasını alır.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Çizgiyi alır.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Grafikteki veri serilerini temsil eden bir [SeriesCollection](../../com.aspose.cells/seriescollection) koleksiyonunu alır.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Grafiğin adını alır.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Bu grafikte sayfa ayarı açıklamasını temsil eder.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Üç\\u9225\\u6178 boyutlu grafik görünümü için perspektifi döndürür veya ayarlar. 0 ile 100 arasında olmalıdır. RightAngleAxes özelliği True ise bu özellik yok sayılır.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Grafikte görünen pivot kontrollerini belirtir

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


Kaynak, pivot tablonun verisidir. PivotSource boş değilse, grafik PivotChart'tır.

**Remarks**

Eğer pivot tablo "PivotTable1", "Sheet1" çalışma sayfasında ve "Book1.xls" dosyasında ise. Grafik ve PivotTable aynı çalışma kitabında değilse pivotSource "[Book1.xls]Sheet1!PivotTable1" olabilir. Bu özelliği ayarlarsanız, önceki veri kaynağı ayarı kaybolur.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder.

Bakınız [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Eksen işaret etiketi etiketlerini içeren grafiğin çizim alanını alır.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Satır ya da sütun bazında çizimin olup olmadığını alır.

Bakınız [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Boş hücrelerin nasıl çizileceğini alır.

Bakınız [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PlotVisibleCellsOnly özelliğini kullanın. Bu yöntem Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Yazdırılan grafik boyutunu alır.

Bakınız [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


Grafik eksenleri dik açıdaysa doğru (True). Yalnızca 3-B grafikler için geçerlidir (Column3D ve 3-B Pasta Grafikleri hariç).

**Remarks**

Bu özellik True ise, Perspective özelliği yok sayılır.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


3B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden).

**Remarks**

Bu özelliğin değeri 0 ile 360 arasında olmalıdır, 3-B çubuk grafikleri dışında; bu grafiklerde değer 0 ile 44 arasında olmalıdır. Varsayılan değer 20'dir. Yalnızca 3-B grafikler için geçerlidir.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Grafiğin ikinci X eksenini alır.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Grafiğin ikinci Y eksenini alır.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Grafiğin seri eksenini alır.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Bu grafikteki tüm çizim şekillerini döndürür.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Grafiğin bir veri tablosu gösterip göstermediğini belirten bir değeri alır.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Grafik açıklamasının (legend) gösterilip gösterilmeyeceğini belirten bir değeri alır. Varsayılan true'dur.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


3B grafiğin yan duvarını temsil eden bir [getWalls()](../../com.aspose.cells/chart\#getWalls--) nesnesini döndürür.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


Microsoft Excel grafiği, grafik sayfası penceresinin boyutuna uyacak şekilde yeniden boyutlandırıyorsa doğru.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Yerleşik stili alır.

**Remarks**

1 ile 48 arasında olmalıdır. Ayarlanmamışsa -1 döndürülür.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Grafiğin alt başlığını alır. Yalnızca ODS dosyalarına uygulanır.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Grafiğin başlığını alır.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Bir grafiğin tipini alır.

Bakın [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Grafiğin Y eksenini alır.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


3B grafiğin duvarlarını temsil eden bir [getWalls()](../../com.aspose.cells/chart\#getWalls--) nesnesini döndürür.

**Remarks**

Bu özellik 3-B pasta grafiklerine uygulanmaz.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


Izgara çizgileri 3B grafikte iki boyutlu olarak çiziliyorsa doğru.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Bu grafiği içeren çalışma sayfasını alır.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Grafikte hangi eksenlerin mevcut olduğunu döndürür.

**Remarks**

Normalde, Pie, PieExploded, PiePie, PieBar, Pie3D, Pie3DExploded, Doughnut, DoughnutExploded eksen içermez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


Grafik tarafından referans verilen hücrenin olup olmadığını döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Sayfa Index.-1, geçerli grafiği içeren çalışma sayfasını ifade eder. |
| rowIndex | int | Satır indeksi |
| columnIndex | int | Sütun indeksi |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Bir grafiğin veri kaynağının değişip değişmediğini algılar.

**Remarks**

Yöntem, grafiği görüntü formatına dönüştürmeden önce grafiğin veri kaynağındaki değişiklikleri algılar. İlk Chart.toImage çağrısında, grafik kaynak verileri (ör. XValuesParseData, ValuesParseData) kaydedilir. Chart.toImage yöntemini tekrar çağırmadan önce, grafiğin yeniden işlenmesi gerekip gerekmediğini kontrol etmek için IsChartDataChanged yöntemini çağırın.

**Returns:**
boolean - Grafik değiştiyse true, aksi takdirde false döndürür.
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Grafik alanının dikdörtgen köşeli olup olmadığını gösteren bir değer alır. Varsayılan değer true'tur.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Hücrenin grafik tarafından referans alınıp alınmadığını döndürür.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen IsCellReferedByChart(int,int,int) yöntemini kullanın. Bu yöntem, Nisan 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi |
| columnIndex | int | Sütun indeksi |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Grafiği belirtilen konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| bottomRow | int | Alt sağ satır indeksi |
| rightColumn | int | Alt sağ sütun indeksi |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


Grafiğin verilerini özet tablo (pivot table) üzerinden yeniler.

**Remarks**

Pivot veri kaynağından pivot tablo raporuna veri toplayacağız. Bu yöntem yalnızca tüm verileri bir pivot grafiğe toplamak için kullanılır.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


Microsoft Excel bir 3-B boyutlu grafiği, eşdeğer 2-B grafiğe daha yakın bir boyuta ölçeklendiriyorsa doğru (True). RightAngleAxes özelliği True olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Grafik için veri aralığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | java.lang.String | Veri serisini çizmek için kullanılacak değerleri belirtir |
| isVertical | boolean | Serileri hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


3-D grafiğin derinliğini, grafik genişliğinin yüzde olarak (20 ile 2000 yüzde arasında) temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


\#N/A değerinin boş olarak gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


3-D grafik görünümünün yüksekliğini derece cinsinden temsil eder.

**Remarks**

Grafik yüksekliği, grafiği gördüğünüz yüksekliği derece cinsinden ifade eder. Çoğu grafik türü için varsayılan değer 15'tir. Bu özelliğin değeri -90 ile 90 arasında olmalıdır, 3-B çubuk grafikleri dışında; bu grafiklerde 0 ile 44 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) ayarlar. Yalnızca pasta, 3D pasta ve halka grafiklerine uygulanır, 0 ile 360 arasında.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


3D grafikte veri serileri arasındaki mesafeyi işaretçi genişliğinin yüzdesi olarak ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Çubuk veya sütun kümeleri arasındaki boşluğu çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


3-D grafiğin yüksekliğini, grafik genişliğinin yüzde olarak (5 ile 500 yüzde arasında) döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Grafik PivotChart olduğunda sadece pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Grafiğin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Üç\\u9225\\u6178 boyutlu grafik görünümü için perspektifi döndürür veya ayarlar. 0 ile 100 arasında olmalıdır. RightAngleAxes özelliği True ise bu özellik yok sayılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


Kaynak, pivot tablonun verisidir. PivotSource boş değilse, grafik PivotChart'tır.

**Remarks**

Eğer pivot tablo "PivotTable1", "Sheet1" çalışma sayfasında ve "Book1.xls" dosyasında ise. Grafik ve PivotTable aynı çalışma kitabında değilse pivotSource "[Book1.xls]Sheet1!PivotTable1" olabilir. Bu özelliği ayarlarsanız, önceki veri kaynağı ayarı kaybolur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder.

Bakınız [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Boş hücrelerin nasıl çizileceğini ayarlar.

Bakınız [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PlotVisibleCellsOnly özelliğini kullanın. Bu yöntem Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Yazdırılan grafik boyutunu ayarlar.

Bakınız [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Grafik alanının dikdörtgen köşeli olup olmadığını gösteren bir değeri ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


Grafik eksenleri dik açıdaysa doğru (True). Yalnızca 3-B grafikler için geçerlidir (Column3D ve 3-B Pasta Grafikleri hariç).

**Remarks**

Bu özellik True ise, Perspective özelliği yok sayılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


3B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden).

**Remarks**

Bu özelliğin değeri 0 ile 360 arasında olmalıdır, 3-B çubuk grafikleri dışında; bu grafiklerde değer 0 ile 44 arasında olmalıdır. Varsayılan değer 20'dir. Yalnızca 3-B grafikler için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Grafiğin veri tablosu gösterip göstermediğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Grafik açıklama kutusunun gösterilip gösterilmeyeceğini belirten bir değeri ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


Microsoft Excel grafiği, grafik sayfası penceresinin boyutuna uyacak şekilde yeniden boyutlandırıyorsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Yerleşik stili ayarlar.

**Remarks**

1 ile 48 arasında olmalıdır. Ayarlanmamışsa -1 döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Bir grafiğin tipini ayarlar.

Bakın [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


Izgara çizgileri 3B grafikte iki boyutlu olarak çiziliyorsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Satır/kolonu değiştirir.

**Returns:**
boolean - False, satır/sütun değiştirme işleminin başarısız olduğunu gösterir.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder.

**Remarks**

Görüntünün formatı `options.ImageFormat` kullanılarak belirtilir. Aşağıdaki formatlar desteklenir: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Daha fazla ayrıntı için lütfen [Supported Charts List][] adresine bakın.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Çıktı akışı. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Ek görüntü oluşturma seçenekleri |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler.

**Remarks**

Görüntünün formatı dosya adının uzantısı kullanılarak belirtilir. Örneğin, "myfile.png" belirtirseniz, görüntü PNG formatında kaydedilir. Aşağıdaki dosya uzantıları tanınır: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | java.lang.String | Tam yol içeren görüntü dosya adı. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Grafik görüntüsünü oluşturur ve belirtilen formatta bir dosyaya kaydeder.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Chart.ToImage(string, ImageType) yöntemini kullanın. Bu özellik, Temmuz 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | java.lang.String | Tam yol içeren görüntü dosya adı. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Görüntünün kaydedileceği format. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler.

**Remarks**

Görüntünün formatı dosya adının uzantısı kullanılarak belirtilir. Örneğin, "myfile.png" belirtirseniz, görüntü PNG formatında kaydedilir. Aşağıdaki dosya uzantıları tanınır: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Daha fazla ayrıntı için lütfen [Supported Charts List][] adresine bakın.

**Example**

300 dpi ve CCITT4 sıkıştırmasıyla Tiff olarak kaydeder.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | java.lang.String | Tam yol içeren görüntü dosya adı. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Ek görüntü oluşturma seçenekleri |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder.

**Remarks**

Görüntünün türü `imageType` kullanılarak belirtilir. Aşağıdaki türler desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | java.lang.String | Tam yol içeren görüntü dosya adı. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). Görüntünün kaydedileceği görüntü türü. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Grafik görüntüsünü oluşturur ve JPEG formatında bir dosyaya kaydeder.

**Remarks**

Genişlik veya yükseklik sıfırsa ya da grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen belirtilen kaliteyle ToImage(string,ImageOrPrintOptions) yöntemini kullanın. Bu yöntem, Mart 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | java.lang.String | Tam yol içeren görüntü dosya adı. |
| jpegQuality | long | Jpeg kalitesi. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Grafik PDF'ini oluşturur ve bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Çıktı akışı. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Grafik PDF'ini oluşturur ve bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Çıktı akışı. |
| desiredPageWidth | float | İstenen sayfa genişliği inç cinsinden. |
| desiredPageHeight | float | İstenen sayfa yüksekliği inç cinsinden. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Çıktı sayfasındaki grafiğin yatay hizalama türü. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Çıktı sayfasındaki grafiğin dikey hizalama türü. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Grafiği bir PDF dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | tam yol ile pdf dosya adı |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Grafiği bir PDF dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | tam yol ile pdf dosya adı |
| desiredPageWidth | float | İstenen sayfa genişliği inç cinsinden. |
| desiredPageHeight | float | İstenen sayfa yüksekliği inç cinsinden. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Çıktı sayfasındaki grafiğin yatay hizalama türü. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Çıktı sayfasındaki grafiğin dikey hizalama türü. |

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

