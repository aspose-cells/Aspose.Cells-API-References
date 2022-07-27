---
title: Chart
second_title: Aspose.Cells for .NET API Referansı
description: Tek bir Excel grafiğini temsil eden nesneyi kapsüller.
type: docs
weight: 430
url: /tr/net/aspose.cells.charts/chart/
---
## Chart class

Tek bir Excel grafiğini temsil eden nesneyi kapsüller.

```csharp
public class Chart
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | Microsoft Excel bir 3-B grafiği, boyut olarak eşdeğer 2-B grafiğe daha yakın olacak şekilde ölçeklendirirse doğrudur. RightAngleAxes özelliği True olmalıdır. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Bir döndürür[`Walls`](./walls) 3 boyutlu grafiğin arka duvarını temsil eden nesne. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Grafiğin X eksenini alır. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Çalışma sayfasındaki grafik alanını alır. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Grafik veri tablosunu temsil eder. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | chartShape'i temsil eder; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | 3B grafiğin derinliğini, grafik genişliğinin yüzdesi olarak temsil eder (yüzde 20 ile 2000 arasında). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | #N/A'nın boş değer olarak görüntülenip görüntülenmeyeceğini belirtir. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Derece olarak 3B harita görünümünün yüksekliğini temsil eder. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | İlk pasta grafiğin veya halka grafik diliminin açısını derece cinsinden (dikeyden saat yönünde) alır veya ayarlar. Yalnızca pasta, 3 boyutlu pasta ve halka grafikler, 0 - 360 için geçerlidir. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Bir döndürür[`Floor`](./floor) 3 boyutlu grafiğin duvarlarını temsil eden nesne. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | 3 boyutlu grafikteki veri serileri arasındaki mesafeyi işaretçi genişliğinin yüzdesi olarak alır veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Çubuk veya sütun genişliğinin yüzdesi olarak çubuk veya sütun kümeleri arasındaki boşluğu döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | 3B grafiğin yüksekliğini grafik genişliğinin yüzdesi olarak döndürür veya ayarlar (yüzde 5 ile 500 arasında). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Pivot grafik alanı düğmelerinin yalnızca grafik PivotChart olduğunda gizlenip gizlenmeyeceğini gösterir. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Grafiğin 3 boyutlu bir grafik olup olmadığını gösterir. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Grafik alanının dikdörtgen köşeli olup olmadığını belirten bir değer alır veya ayarlar. Varsayılan değer true'dur. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Grafik göstergesini alır. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Satırı alır. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Grafiğin adını alır ve ayarlar. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | [`SeriesCollection`](../seriescollection) grafikteki veri serilerini temsil eden koleksiyon. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Bu çizelgedeki sayfa düzeni açıklamasını temsil eder. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | 3 boyutlu tablo görünümünün perspektifini döndürür veya ayarlar. 0 ile 100 arasında olmalıdır. RightAngleAxes özelliği True ise bu özellik yoksayılır. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | chart üzerinde görünen pivot kontrollerini belirtir |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | Kaynak, pivotTable'ın verileridir. PivotSource boş değilse, grafik PivotChart'tır. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Grafiğin altındaki hücrelere eklenme şeklini temsil eder. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Eksen onay etiketlerini içeren grafiğin çizim alanını alır. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Satıra mı yoksa sütuna göre mi çizileceğini alır ve ayarlar. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Boş hücrelerin nasıl çizileceğini alır ve ayarlar. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Yalnızca görünür hücrelerin çizilip çizilmediğini gösterir. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Yazdırılan grafik boyutunu alır ve ayarlar. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Grafik eksenleri dik açıdaysa doğrudur. Yalnızca 3B grafikler için geçerlidir(Sütun3B ve 3B Pasta Grafikler hariç). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | 3B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Grafiğin ikinci X eksenini alır. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Grafiğin ikinci Y eksenini alır. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Grafiğin seri eksenini alır. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Bu grafikteki tüm çizim şekillerini döndürür. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Grafiğin bir veri tablosu gösterip göstermediğini gösteren bir değer alır veya ayarlar. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Grafik göstergesinin gösterilip gösterilmeyeceğini belirten bir değer alır veya ayarlar. Varsayılan true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Bir döndürür[`Walls`](./walls) boyutlu grafiğin yan duvarını temsil eden nesne. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Microsoft Excel grafiği, grafik sayfası penceresinin boyutuna uyacak şekilde yeniden boyutlandırırsa doğrudur. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Yerleşik stili alır ve ayarlar. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Grafiğin alt başlığını alır. Yalnızca ODS biçim dosyası için. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Grafiğin başlığını alır. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Bir grafiğin türünü alır veya ayarlar. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Grafiğin Y eksenini alır. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Bir döndürür[`Walls`](./walls) 3 boyutlu grafiğin duvarlarını temsil eden nesne. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Kılavuz çizgileri 3 boyutlu bir grafikte iki boyutlu olarak çizilirse doğrudur. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Bu grafiği içeren çalışma sayfasını alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Çizim alanının özel konumunu hesaplar, konumları otomatik olarak atanmışsa eksenler. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Grafiğin gerçek boyutunu piksel birimi olarak alır. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Grafiğin veri kaynağı aralığını alır. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Grafikte hangi eksenlerin bulunduğunu döndürür. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Bir grafiğin veri kaynağının değişip değişmediğini algılar. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Grafiği belirtilen bir konuma taşır. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Özet veri kaynağındaki özet grafiğin verilerini yeniler. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Bir grafik için veri aralığını belirtir. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Satır/sütun arasında geçiş yapar. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | 32-bit alır`bit eşlem` grafiğin nesnesi. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | 32 bit alır`bit eşlem` grafiğin nesnesi. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression ve ImageOrPrintOptions.Quality nitelikleri yok sayılır. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün biçimini belirler. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | Grafik görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | Grafik görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | Grafik görüntüsünü oluşturur ve onu Jpeg biçiminde bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün biçimini belirler. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | Grafik görüntüsünü oluşturur ve Jpeg biçiminde bir dosyaya kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Grafik pdf'sini oluşturur ve bir akışa kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Grafiği bir pdf dosyasına kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Grafik pdf'sini oluşturur ve bir akışa kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Grafiği bir pdf dosyasına kaydeder. |

### Örnekler

```csharp
[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
