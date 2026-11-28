---
title: "Sınıf Chart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.Chart sınıfı. Tek bir Excel grafiğini temsil eden nesneyi kapsüller."
type: docs
url: /tr/net/aspose.cells.charts/chart/
---
## Chart class

Tek bir Excel grafiğini temsil eden nesneyi kapsar.

```csharp
public class Chart
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Grafiğin gerçek boyutunu piksel biriminde alır. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | Microsoft Excel bir 3D grafiği, eşdeğer 2D grafiğe boyut olarak daha yakın olacak şekilde ölçeklendiriyorsa True. RightAngleAxes özelliği True olmalıdır. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | 3D grafiğin arka duvarını temsil eden bir [`Walls`](./walls/) nesnesi döndürür. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Grafiğin X eksenini alır. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Çalışma sayfasındaki grafik alanını alır. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Grafik veri tablosunu temsil eder. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | chartShape öğesini temsil eder; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | 3‑D bir grafiğin derinliğini, grafik genişliğinin yüzdesi olarak temsil eder (20 ile 2000 yüzde arasında). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | #N/A değerinin boş bir değer olarak gösterilip gösterilmeyeceğini belirtir. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | 3‑D grafik görünümünün yüksekliğini derece cinsinden temsil eder. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Grafikte filtrelenen veri serilerini temsil eden bir [`SeriesCollection`](../seriescollection/) koleksiyonu alır. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden alır veya ayarlar (dikeyden saat yönünde). Yalnızca pasta, 3‑D pasta ve halka grafiklerinde uygulanır, 0 ile 360 arasında. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | 3‑D grafiğin duvarlarını temsil eden bir [`Floor`](./floor/) nesnesi döndürür. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | 3‑D grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzdesi olarak alır veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | 3‑D grafiğin yüksekliğini, grafik genişliğinin yüzdesi olarak döndürür veya ayarlar (5 ile 500 yüzde arasında). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Grafik PivotChart olduğunda yalnızca pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini belirtir. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Grafiğin 3D grafik olup olmadığını belirtir. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Grafik alanının dikdörtgen köşeli olup olmadığını belirten bir değeri alır veya ayarlar. Varsayılan true'dur. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Grafik açıklamasını alır. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Çizgiyi alır. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Grafiğin adını alır ve ayarlar. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Grafikteki veri serilerini temsil eden bir [`SeriesCollection`](../seriescollection/) koleksiyonu alır. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Bu grafikteki sayfa ayarı açıklamasını temsil eder. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Üç boyutlu grafik görünümü için perspektifi döndürür veya ayarlar. 0 ile 100 arasında olmalıdır. RightAngleAxes özelliği True ise bu özellik yok sayılır. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Grafikte görünen pivot kontrollerini belirtir. |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | Kaynak, pivot tablosunun verisidir. PivotSource boş değilse, grafik PivotChart'tır. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Eksen işaret etiketi etiketlerini içeren grafiğin çizim alanını alır. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Satır veya sütun bazında çizim yapılıp yapılmayacağını alır ve ayarlar. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Boş hücrelerin nasıl çizileceğini alır ve ayarlar. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Sadece çizim görünür hücrelerini gösterip göstermediğini belirtir. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Çizim görünür hücrelerini yalnızca gösterip göstermediğini belirtir. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Yazdırılan grafik boyutunu alır ve ayarlar. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | Grafik eksenleri dik açıdaysa True. Yalnızca 3-B grafikler için geçerlidir (Column3D ve 3-B Pasta Grafikleri hariç). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | 3-B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Grafiğin ikinci X eksenini alır. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Grafiğin ikinci Y eksenini alır. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Grafiğin seri eksenini alır. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Bu grafikteki tüm çizim şekillerini döndürür. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Grafiğin veri tablosu gösterip göstermediğini belirten bir değeri alır veya ayarlar. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Grafik açıklamasının gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | 3-B grafiğin yan duvarını temsil eden bir [`Walls`](./walls/) nesnesini döndürür. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | Microsoft Excel, grafiği grafik sayfası penceresinin boyutuna göre yeniden boyutlandırıyorsa True. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Yerleşik stili alır ve ayarlar. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Grafiğin alt başlığını alır. Yalnızca ODS dosyalarına uygulanır. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Grafiğin başlığını alır. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Bir grafiğin tipini alır veya ayarlar. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Grafiğin Y eksenini alır. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | 3-B grafiğin duvarlarını temsil eden bir [`Walls`](./walls/) nesnesini döndürür. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | Izgara çizgileri 3-B grafikte iki boyutlu olarak çiziliyorsa True. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Bu grafiği içeren çalışma sayfasını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Çizim alanı ve eksenlerin konumları otomatik atanmışsa, özel konumlarını hesaplar. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Grafik Hesaplama Seçenekleri ile, çizim alanı ve eksenlerin konumu otomatik atanmışsa, özel konumlarını hesaplar. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Önceden ayarlanmış bir şablonla grafik tipini değiştir. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Grafiğin gerçek boyutunu piksel biriminde alır. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Grafiğin veri kaynağı aralığını alır. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Grafikte mevcut olan eksenleri döndürür. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Grafik tarafından referans verilen hücrenin var olup olmadığını döndürür. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Bir grafiğin veri kaynağının değişip değişmediğini algılar. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Eski.**) Grafik tarafından referans verilen hücrenin var olup olmadığını döndürür. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Grafiği belirtilen konuma taşır. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Grafiğin verilerini özet tablodan yeniler. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Grafik için veri aralığını belirtir. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Satır/sütunu değiştirir. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Grafiğin 32-bit `Bitmap` nesnesini alır. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Grafiğin 32-bit `Bitmap` nesnesini alır. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression ve ImageOrPrintOptions.Quality öznitelikleri göz ardı edilir. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Eski.**) Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Grafik görüntüsünü oluşturur ve Jpeg formatında bir akışa kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Eski.**) Grafik görüntüsünü oluşturur ve belirtilen formatta bir dosyaya kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Eski.**) Grafik görüntüsünü oluşturur ve Jpeg formatında bir dosyaya kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Grafik PDF'ini oluşturur ve bir akışa kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Grafiği bir pdf dosyasına kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Grafik pdf'ini oluşturur ve bir akışa kaydeder. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Grafiği bir pdf dosyasına kaydeder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarlayın
            chart.SetChartDataRange("A1:B4", true);

            // Grafik özelliklerini ayarla
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Grafiğin görünümünü özelleştir
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Grafiğin eksenlerini özelleştir
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Grafiğin lejantını özelleştir
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Grafiğin çizim alanını özelleştir
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Grafiğin grafik alanını özelleştir
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


