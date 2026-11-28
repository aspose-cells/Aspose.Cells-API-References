---
title: "Sınıf ImageOrPrintOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.ImageOrPrintOptions sınıfı. Çalışma sayfasını görüntülere render ederken, çalışma sayfasını yazdırırken veya grafiği görüntüye render ederken seçenekleri belirtmeye olanak tanır."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Çalışma sayfasını görüntülere oluştururken, çalışma sayfasını yazdırırken veya grafiği görüntüye oluştururken seçenekleri belirtmeye izin verir.

```csharp
public class ImageOrPrintOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt genişliği geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Dönüştürürken grafik görüntü tipini belirtin. varsayılan değer: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf, görüntüde blok olarak görünebilirler. Bu değeri true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipini kullanarak bu karakterleri göstermeye çalışır. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | İstemci, bu EventHandler'ı kullanarak her sayfayı yazdırırken özel bir çıktı alabilir. |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | İstemci, bu EventHandler'ı kullanarak her sayfayı yazdırırken yazıcının sayfa ayarlarını kontrol edebilir. |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Renderleme sırasında özel ayarları alır veya ayarlar. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Varsayılan düzenleme dilini alır veya ayarlar. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir DefaultFont ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Renderleme sırasında DrawObject ve Bound elde etmek için bu arabirimi uygular. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) SVG içinde gömülü görüntünün dosya adını belirtin. Bu, "c:\\xpsEmbedded" gibi bir dizinle tam yol olmalıdır. |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Kaynak dosyada Emf metafile'lerinin render edilmesi için ayar. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Metafile formatını belirten bir EmfType alır veya ayarlar. Varsayılan değer EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Izgara çizgi rengini alır veya ayarlar. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Izgara çizgi tipini alır veya ayarlar. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Oluşturulan görüntüler için yatay çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Oluşturulan görüntülerin formatını alır veya ayarlar. Varsayılan değer: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Çıktı öğelerinin optimize edilip edilmediğini gösterir. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. Sayfa ayarının kağıt boyutu geçersiz olacak ve sayfa ayarının diğer ayarları hâlâ geçerli olacaktır. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Bu özellik true ise, bir Alan çıktılanır ve ölçekleme etkili olmaz. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır veya ayarlar. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Sayfa kaydetme işleminin ilerlemesini kontrol/indike eder. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Oluşturulan görüntüler için piksel formatını alır veya ayarlar. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Hangi sayfaların yazdırılmayacağını gösterir. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir. Aksi takdirde böyle bir iletişim kutusu gösterilmez. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Sayfaları `Jpeg` formatında kaydederken uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar. Varsayılan değer 100. |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Çıktı dosya formatı türünü alır veya ayarlar. Tiff/XPS desteklenir. |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Düzleştirme (antialiasing) işleminin çizgilere, eğrilere ve doldurulmuş alanların kenarlarına uygulanıp uygulanmayacağını belirtir. Varsayılan değer SmoothingMode.None'dur. |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) SVG'deki css adının önekini alır ve ayarlar, varsayılan değer boş dizedir. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) Bu özellik true ise, oluşturulan svg görünüm alanına sığacaktır. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin tipini alır veya ayarlar. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Metin renderleme kalitesini belirtir. Varsayılan değer TextRenderingHint.SystemDefault'dur. |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | [`ImageType`](./imagetype/) Tiff ve [`TiffCompression`](./tiffcompression/) Ccitt3 veya Ccitt4 olduğunda, görüntüleri 1 bpp formatına dönüştürürken kullanılan yöntemi alır veya ayarlar. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | `Tiff` formatına sayfalar kaydedilirken yalnızca uygulanacak bit derinliğini alır veya ayarlar. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | `Tiff` formatına sayfalar kaydedilirken yalnızca uygulanacak sıkıştırma türünü alır veya ayarlar. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Oluşturulan görüntüler için dikey çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Görüntünün istenen genişlik ve yüksekliğini ayarlar. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Görüntünün istenen genişlik ve yüksekliğini ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // ImageOrPrintOptions oluşturun ve özellikleri ayarlayın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Örnek veri ve grafik içeren yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği seçenekleri kullanarak görüntü olarak kaydedin
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


