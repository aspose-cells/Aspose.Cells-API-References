---
title: "Series"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir grafikte tek bir veri serisini temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Bir grafikte tek bir veri serisini temsil eden nesneyi kapsüller.

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
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Series nesnesinin arka plan alanını temsil eder. |
| [getBar3DShapeType()](#getBar3DShapeType--) | 3D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini alır. |
| [getBorder()](#getBorder--) | Series nesnesinin kenarlığını temsil eder. |
| [getBubbleScale()](#getBubbleScale--) | Belirtilen grafik grubundaki balonlar için ölçek faktörünü alır. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Balon grafiğinde balon boyutunun neyi temsil ettiğini alır. |
| [getBubbleSizes()](#getBubbleSizes--) | Grafik serisinin balon boyut değerlerini alır. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Seri için önbelleğe alınmış kategori değerlerini alır. |
| [getCachedValues()](#getCachedValues--) | Seri için önbelleğe alınmış değerleri alır. |
| [getCategoryValues()](#getCategoryValues--) | Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek kategori değerlerini alır. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Veri değerlerinin sayısını alır. |
| [getDataLabels()](#getDataLabels--) | Belirtilen ASeries için DataLabels nesnesini temsil eder. |
| [getDisplayName()](#getDisplayName--) | Grafik üzerinde gösterilen serinin adını alır. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. |
| [getDownBars()](#getDownBars--) | Bir çizgi grafiğindeki aşağı çubukları temsil eden bir [DropBars](../../com.aspose.cells/dropbars) nesnesi döndürür. |
| [getDropLines()](#getDropLines--) | Bir çizgi grafiği veya alan grafiğinde bir serinin düşen çizgilerini temsil eden bir [Line](../../com.aspose.cells/line) nesnesi döndürür. |
| [getExplosion()](#getExplosion--) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) alır. |
| [getGapWidth()](#getGapWidth--) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzde olarak döndürür veya ayarlar. |
| [getHas3DEffect()](#getHas3DEffect--) | Seri üç boyutlu bir görünüme sahipse true. |
| [getHiLoLines()](#getHiLoLines--) | Bir çizgi grafiğinde bir serinin yüksek-düşük çizgilerini temsil eden bir HiLoLines nesnesi döndürür. |
| [getLayoutProperties()](#getLayoutProperties--) | Düzenin özelliklerini temsil eder. |
| [getLeaderLines()](#getLeaderLines--) | Grafikteki lider çizgileri temsil eder. |
| [getLegendEntry()](#getLegendEntry--) | Bu seriye göre lejand girişini alır. |
| [getMarker()](#getMarker--) | Alır [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Veri serisinin adını alır. |
| [getOverlap()](#getOverlap--) | Çubukların ve sütunların nasıl konumlandırıldığını belirtir. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir. |
| [getPointValues()](#getPointValues--) | Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek değerleri alır. |
| [getPoints()](#getPoints--) | Grafikte bir serideki nokta koleksiyonunu alır. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Bir pasta içinde pasta grafiği ya da pasta içinde çubuk grafiğinin ikincil bölümünün boyutunu, birincil pastanın boyutunun yüzdesi olarak döndürür veya ayarlar. |
| [getSeriesLines()](#getSeriesLines--) | Yığılmış çubuk grafiği veya yığılmış sütun grafiği için seri çizgilerini temsil eden bir SeriesLines nesnesi döndürür. |
| [getShadow()](#getShadow--) | Serinin bir gölgesi varsa doğru. |
| [getShapeProperties()](#getShapeProperties--) | Serinin görsel şekil özelliklerini tutan [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) nesnesini alır. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | Grafik grubunda negatif baloncuklar gösteriliyorsa doğru. |
| [getSizeRepresents()](#getSizeRepresents--) | Balon grafiğinde balon boyutunun neyi temsil ettiğini alır. |
| [getSmooth()](#getSmooth--) | Eğri yumuşatmayı temsil eder. |
| [getSplitType()](#getSplitType--) | Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için bir değeri döndürür veya ayarlar. |
| [getSplitValue()](#getSplitValue--) | Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için kullanılacak bir değeri döndürür veya ayarlar. |
| [getTrendLines()](#getTrendLines--) | Bu serinin tüm eğri çizgilerini döndürür. |
| [getType()](#getType--) | Bir veri serisinin tipini alır. |
| [getUpBars()](#getUpBars--) | Bir çizgi grafiğindeki yükselen çubukları temsil eden bir DropBars nesnesi döndürür. |
| [getValues()](#getValues--) | Bu grafik serisinin Y değerlerini temsil eder. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Values NumberList'in format kodunu temsil eder. |
| [getXErrorBar()](#getXErrorBar--) | Serinin X yönündeki hata çubuğunu temsil eder. |
| [getXValues()](#getXValues--) | Bu grafik serisinin X değerlerini temsil eder. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | X Values' NumberList'in format kodunu temsil eder. |
| [getYErrorBar()](#getYErrorBar--) | Serinin Y yönündeki hata çubuğunu temsil eder. |
| [hasDropLines()](#hasDropLines--) | Grafiğin düşen çizgileri varsa doğru. |
| [hasHiLoLines()](#hasHiLoLines--) | Çizgi grafiğinin yüksek-düşük çizgileri varsa doğru. |
| [hasLeaderLines()](#hasLeaderLines--) | Serinin lider çizgileri varsa doğru. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | Radar grafiğinin kategori eksen etiketleri varsa doğru. |
| [hasSeriesLines()](#hasSeriesLines--) | Doğru, yığılmış sütun grafik veya çubuk grafik seriler çizgilerine sahipse veya Pie of Pie grafiği ya da Bar of Pie grafiği iki bölüm arasında bağlayıcı çizgilere sahipse. |
| [hasUpDownBars()](#hasUpDownBars--) | Doğru, bir çizgi grafiğinde yukarı ve aşağı çubuklar varsa. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Eşik değerinin otomatik olup olmadığını gösterir. |
| [isColorVaried()](#isColorVaried--) | Nokta renklerinin değişken olup olmadığını temsil eder. |
| [isFiltered()](#isFiltered--) | Serinin seçili mi yoksa filtrelenmiş mi olduğunu gösterir. |
| [isVerticalValues()](#isVerticalValues--) | Veri kaynağının dikey olup olmadığını gösterir. |
| [move(int count)](#move-int-) | Seriyi yukarı ya da aşağı hareket ettirir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | 3‑D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini ayarlar. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Belirtilen grafik grubundaki balonlar için ölçek faktörünü ayarlar. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Balon grafiğinde balon boyutunun neyi temsil ettiğini alır. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Grafik serisinin balon boyutu değerlerini ayarlar. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Nokta renklerinin değişken olup olmadığını temsil eder. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. |
| [setExplosion(int value)](#setExplosion-int-) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Serinin seçili mi yoksa filtrelenmiş mi olduğunu gösterir. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden ayarlar (dikeyden saat yönünde). |
| [setGapWidth(short value)](#setGapWidth-short-) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzde olarak döndürür veya ayarlar. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | Seri üç boyutlu bir görünüme sahipse true. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | Grafiğin düşen çizgileri varsa doğru. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | Çizgi grafiğinin yüksek-düşük çizgileri varsa doğru. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | Serinin lider çizgileri varsa doğru. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | Radar grafiğinin kategori eksen etiketleri varsa doğru. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Doğru, yığılmış sütun grafik veya çubuk grafik seriler çizgilerine sahipse veya Pie of Pie grafiği ya da Bar of Pie grafiği iki bölüm arasında bağlayıcı çizgilere sahipse. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Doğru, bir çizgi grafiğinde yukarı ve aşağı çubuklar varsa. |
| [setName(String value)](#setName-java.lang.String-) | Veri serisinin adını ayarlar. |
| [setOverlap(short value)](#setOverlap-short-) | Çubukların ve sütunların nasıl konumlandırıldığını belirtir. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Bir pasta içinde pasta grafiği ya da pasta içinde çubuk grafiğinin ikincil bölümünün boyutunu, birincil pastanın boyutunun yüzdesi olarak döndürür veya ayarlar. |
| [setShadow(boolean value)](#setShadow-boolean-) | Serinin bir gölgesi varsa doğru. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | Grafik grubunda negatif baloncuklar gösteriliyorsa doğru. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Balon grafiğinde balon boyutunun neyi temsil ettiğini ayarlar. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Eğri yumuşatmayı temsil eder. |
| [setSplitType(int value)](#setSplitType-int-) | Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için bir değeri döndürür veya ayarlar. |
| [setSplitValue(double value)](#setSplitValue-double-) | Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için kullanılacak bir değeri döndürür veya ayarlar. |
| [setType(int value)](#setType-int-) | Bir veri serisinin tipini ayarlar. |
| [setValues(String value)](#setValues-java.lang.String-) | Bu grafik serisinin Y değerlerini temsil eder. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Values NumberList'in format kodunu temsil eder. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Bu grafik serisinin X değerlerini temsil eder. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | X Values' NumberList'in format kodunu temsil eder. |
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


Series nesnesinin arka plan alanını temsil eder.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


3D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini alır.

Bakınız [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Series nesnesinin kenarlığını temsil eder.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Belirtilen grafik grubundaki balonlar için ölçek faktörünü alır. 0 (sıfır) ile 300 arasında bir tam sayı değer olabilir ve varsayılan boyutun yüzdesine karşılık gelir. Yalnızca balon grafiklerinde uygulanır.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Balon grafiğinde balon boyutunun neyi temsil ettiğini alır.

Bakınız [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Aspose.Cells.Charts.Series.SizeRepresents özelliğini kullanın. Bu özellik OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Grafik serisinin balon boyut değerlerini alır.

**Remarks**

Yalnızca [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) veya [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) için.

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Seri için önbelleğe alınmış kategori değerlerini alır.

**Remarks**

NOT: Bu özellik şu anda yalnızca dahili kullanım içindir. Bir sonraki sürümde değiştirilecek veya kaldırılacaktır.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Seri için önbelleğe alınmış değerleri alır.

**Remarks**

NOT: Bu özellik şu anda yalnızca dahili kullanım içindir. Bir sonraki sürümde değiştirilecek veya kaldırılacaktır.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek kategori değerlerini alır.

**Remarks**

Bu özellik, özellikle belirtilen veri kaynağı dış bağlantı, formül vb. olduğunda, [getXValues()](../../com.aspose.cells/series\#getXValues--) tarafından tanımlanan verilere karşılık gelen gerçek değerleri almanın pratik bir yolunu sunar.

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


Veri değerlerinin sayısını alır.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Belirtilen ASeries için DataLabels nesnesini temsil eder.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Grafik üzerinde gösterilen serinin adını alır.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. Delik boyutu, grafik boyutunun yüzde olarak 10 ile 90 arasında bir değeri olarak ifade edilir.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Bir çizgi grafiğindeki aşağı çubukları temsil eden bir [DropBars](../../com.aspose.cells/dropbars) nesnesi döndürür. Yalnızca çizgi grafiklerinde uygulanır.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Çizgi grafiği veya alan grafiğindeki bir serinin düşen çizgilerini temsil eden bir [Line](../../com.aspose.cells/line) nesnesi döndürür. Yalnızca çizgi grafiklerinde veya alan grafiklerinde uygulanır.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) alır. Yalnızca pasta, 3‑D pasta ve halka grafiklerinde uygulanır; değerler 0 ile 360 arasındadır.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Çubuk veya sütun kümeleri arasındaki boşluğu çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


Seri üç boyutlu bir görünüme sahipse true.

**Remarks**

Yalnızca [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) veya [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) grafiklerine uygulanır.

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Bir satır grafiğindeki serinin yüksek-düşük çizgilerini temsil eden bir HiLoLines nesnesi döndürür. Yalnızca satır grafiklerine uygulanır.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Düzenin özelliklerini temsil eder.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Bir grafikte lider çizgileri temsil eder. Lider çizgileri veri etiketlerini veri noktalarına bağlar. Bu nesne bir koleksiyon değildir; tek bir lider çizgiyi temsil eden bir nesne yoktur.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Bu seriye göre lejand girişini alır.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Alır [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Veri serisinin adını alır.

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


Çubukların ve sütunların nasıl konumlandırıldığını belirtir. -100 ile 100 arasında bir değer olabilir. Yalnızca 2D çubuk ve 2D sütun grafiklerine uygulanır.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek değerleri alır.

**Remarks**

Bu özellik, özellikle belirtilen veri kaynağı harici bağlantı, formül vb. olduğunda, [getValues()](../../com.aspose.cells/series\#getValues--) tarafından tanımlanan verilere karşılık gelen gerçek değerleri almanın pratik bir yolunu sağlar.

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


Grafikte bir serideki nokta koleksiyonunu alır.

**Remarks**

Grafik Pie of Pie veya Bar of Pie olduğunda, son nokta ilk pasta çizimindeki diğer nokta olur.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Bir pie of pie grafiği veya bar of pie grafiğinin ikincil bölümünün boyutunu, birincil pastanın boyutuna yüzde olarak döndürür veya ayarlar. 5 ile 200 arasında bir değer olabilir.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Yığılmış çubuk grafiği veya yığılmış sütun grafiği için seri çizgilerini temsil eden bir SeriesLines nesnesi döndürür. Yalnızca yığılmış çubuk ve yığılmış sütun grafiklerine uygulanır.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Serinin bir gölgesi varsa doğru.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Serinin görsel şekil özelliklerini tutan [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) nesnesini alır.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


Grafik grubu için negatif baloncuklar gösteriliyorsa doğru (true). Yalnızca baloncuk grafiklerinde geçerlidir.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Balon grafiğinde balon boyutunun neyi temsil ettiğini alır.

Bakınız [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea, [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) değerinin balonun alanı olduğu anlamına gelir. BubbleSizeRepresents.SizeIsWidth ise [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) değerinin balonun genişliği olduğu anlamına gelir.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Eğri yumuşatmayı temsil eder. Satır grafiği veya dağılım grafiği için eğri yumuşatma etkinse doğru (true). Yalnızca satır grafikleri ve çizgili dağılım grafiklerine uygulanır.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için bir değeri döndürür veya ayarlar.

[ChartSplitType](../../com.aspose.cells/chartsplittype) bakınız.

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için kullanılacak bir değeri döndürür veya ayarlar.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Bu serinin tüm eğri çizgilerini döndürür.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Bir veri serisinin tipini alır.

Bakın [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Bir satır grafiğindeki yukarı çubukları temsil eden bir DropBars nesnesi döndürür. Yalnızca satır grafiklerine uygulanır.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Bu grafik serisinin Y değerlerini temsil eder.

**Remarks**

Bu özellik tarafından tanımlanan gerçek değerleri (bu serinin her noktasına karşılık gelen) almak için lütfen [getPointValues()](../../com.aspose.cells/series\#getPointValues--) kullanın.

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Values NumberList'in format kodunu temsil eder.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Serinin X yönündeki hata çubuğunu temsil eder.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Bu grafik serisinin X değerlerini temsil eder.

**Remarks**

Yalnızca Dağılım ve Baloncuk grafikleri için. Diğer grafik türleri için lütfen [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) kullanın. [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) bu serinin gerçek kategori değerlerini almak için kullanılır.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


X Values' NumberList'in format kodunu temsil eder.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Serinin Y yönündeki hata çubuğunu temsil eder.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


Grafikte düşen çizgiler varsa doğru (true). Yalnızca satır grafiği veya alan grafiklerine uygulanır.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


Satır grafiğinde yüksek-düşük çizgileri varsa doğru (true). Yalnızca satır grafiklerine uygulanır.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


Serinin lider çizgileri varsa doğru.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


Radar grafiğinde kategori ekseni etiketleri varsa doğru (true). Yalnızca radar grafiklerine uygulanır.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


Yığılmış sütun grafiği veya çubuk grafiğinde seri çizgileri varsa veya Pie of Pie grafiği ya da Bar of Pie grafiğinde iki bölüm arasında bağlayıcı çizgiler varsa doğru (true). Yalnızca yığılmış sütun grafikleri, çubuk grafikleri, Pie of Pie grafikleri veya Bar of Pie grafiklerine uygulanır.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


Satır grafiğinde yukarı ve aşağı çubukları varsa doğru (true). Yalnızca satır grafiklerine uygulanır.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


Eşik değerinin otomatik olup olmadığını gösterir.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Noktaların renginin değişken olup olmadığını temsil eder. Grafik yalnızca bir seri içermeli veya bu grafik bir pasta grafiği olmalıdır.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Serinin seçili mi yoksa filtrelenmiş mi olduğunu gösterir. Doğru (true) bu serinin filtrelendiğini ve grafikte gösterilmeyeceğini belirtir.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Veri kaynağının dikey olup olmadığını gösterir.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Seriyi yukarı ya da aşağı hareket ettirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayı | int | Yukarı veya aşağı hareket sayısı. Bu değer sıfırdan küçükse seriyi yukarı taşı; sıfırdan büyükse seriyi aşağı taşı. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


3‑D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini ayarlar.

Bakınız [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Belirtilen grafik grubundaki baloncuklar için ölçek faktörünü ayarlar. Varsayılan boyutun yüzde karşılığı olarak 0 (sıfır) ile 300 arasında bir tamsayı değer olabilir. Yalnızca baloncuk grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Balon grafiğinde balon boyutunun neyi temsil ettiğini alır.

Bakınız [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Aspose.Cells.Charts.Series.SizeRepresents özelliğini kullanın. Bu özellik OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Grafik serisinin balon boyutu değerlerini ayarlar.

**Remarks**

Yalnızca [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) veya [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Noktaların renginin değişken olup olmadığını temsil eder. Grafik yalnızca bir seri içermeli veya bu grafik bir pasta grafiği olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. Delik boyutu, grafik boyutunun yüzde olarak 10 ile 90 arasında bir değeri olarak ifade edilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Serinin seçili mi yoksa filtrelenmiş mi olduğunu gösterir. Doğru (true) bu serinin filtrelendiğini ve grafikte gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) ayarlar. Yalnızca pasta, 3D pasta ve halka grafiklerinde uygulanır ve değerler 0 ile 360 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Çubuk veya sütun kümeleri arasındaki boşluğu çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


Seri üç boyutlu bir görünüme sahipse true.

**Remarks**

Yalnızca [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) veya [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


Grafikte düşen çizgiler varsa doğru (true). Yalnızca satır grafiği veya alan grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


Satır grafiğinde yüksek-düşük çizgileri varsa doğru (true). Yalnızca satır grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


Serinin lider çizgileri varsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


Radar grafiğinde kategori ekseni etiketleri varsa doğru (true). Yalnızca radar grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


Yığılmış sütun grafiği veya çubuk grafiğinde seri çizgileri varsa veya Pie of Pie grafiği ya da Bar of Pie grafiğinde iki bölüm arasında bağlayıcı çizgiler varsa doğru (true). Yalnızca yığılmış sütun grafikleri, çubuk grafikleri, Pie of Pie grafikleri veya Bar of Pie grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


Satır grafiğinde yukarı ve aşağı çubukları varsa doğru (true). Yalnızca satır grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Veri serisinin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Çubukların ve sütunların nasıl konumlandırıldığını belirtir. -100 ile 100 arasında bir değer olabilir. Yalnızca 2D çubuk ve 2D sütun grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Bir pie of pie grafiği veya bar of pie grafiğinin ikincil bölümünün boyutunu, birincil pastanın boyutuna yüzde olarak döndürür veya ayarlar. 5 ile 200 arasında bir değer olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Serinin bir gölgesi varsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


Grafik grubu için negatif baloncuklar gösteriliyorsa doğru (true). Yalnızca baloncuk grafiklerinde geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Balon grafiğinde balon boyutunun neyi temsil ettiğini ayarlar.

Bakınız [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea, [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) değerinin balonun alanı olduğu anlamına gelir. BubbleSizeRepresents.SizeIsWidth ise [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) değerinin balonun genişliği olduğu anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Eğri yumuşatmayı temsil eder. Satır grafiği veya dağılım grafiği için eğri yumuşatma etkinse doğru (true). Yalnızca satır grafikleri ve çizgili dağılım grafiklerine uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için bir değeri döndürür veya ayarlar.

[ChartSplitType](../../com.aspose.cells/chartsplittype) bakınız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Bir pasta içinde pasta veya pasta içinde çubuk grafiğinde hangi veri noktalarının ikinci pasta veya çubukta olduğunu belirlemek için kullanılacak bir değeri döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Bir veri serisinin tipini ayarlar.

Bakın [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Bu grafik serisinin Y değerlerini temsil eder.

**Remarks**

Bu özellik tarafından tanımlanan gerçek değerleri (bu serinin her noktasına karşılık gelen) almak için lütfen [getPointValues()](../../com.aspose.cells/series\#getPointValues--) kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Values NumberList'in format kodunu temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Bu grafik serisinin X değerlerini temsil eder.

**Remarks**

Yalnızca Dağılım ve Baloncuk grafikleri için. Diğer grafik türleri için lütfen [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) kullanın. [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) bu serinin gerçek kategori değerlerini almak için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


X Values' NumberList'in format kodunu temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

