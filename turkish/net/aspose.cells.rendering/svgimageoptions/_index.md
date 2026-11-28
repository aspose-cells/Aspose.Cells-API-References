---
title: "Sınıf SvgImageOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.SvgImageOptions sınıfı. Svg görüntüsü oluşturmak için seçenekler"
type: docs
url: /tr/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Svg görüntüsü oluşturma seçenekleri.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği yalnızca bir sayfaya çıktılanır. Sayfa ayarı (pagesetup) genişliği geçersiz olur ve pagesetup'ın diğer ayarları hâlâ etkili olur. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Dönüştürürken grafik görüntü türünü belirtir. varsayılan değer: PNG. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. Bunu true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipini kullanarak bu karakterleri göstermeye çalışır. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Svg içinde css adının önekini alır ve ayarlar, varsayılan değer boş dizedir. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | İstemci, her sayfayı bu EventHandler kullanarak yazıcıya özel çıktı verebilir (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | İstemci, her sayfayı bu EventHandler kullanarak yazıcının sayfa ayarlarını kontrol edebilir (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Render sırasında özel ayarları alır veya ayarlar. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Varsayılan düzenleme dilini alır veya ayarlar. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için DefaultFont'u MingLiu veya MS Gothic gibi bir değerle ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanır. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Render sırasında DrawObject ve Bound elde etmek için bu arabirimi uygular. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Svg'ye gömülen yazı tipi türünü alır veya ayarlar. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Svg içinde gömülü görüntünün dosya adını belirtir. Bu, "c:\\xpsEmbedded" gibi bir dizin içeren tam yol olmalıdır (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Kaynak dosyadaki Emf metafile'lerini renderlemek için ayar. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Metafile formatını belirten bir EmfType alır veya ayarlar. Varsayılan değer EmfPlusDual'dir. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Bu özellik true ise, oluşturulan svg görüntüleme alanına sığar. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Izgara çizgi rengini alır veya ayarlar. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Izgara çizgi tipini alır veya ayarlar. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Oluşturulan görüntüler için yatay çözünürlüğü DPI cinsinden alır veya ayarlar. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Oluşturulan görüntülerin formatını alır veya ayarlar. Varsayılan değer: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmayacağını gösterir. Varsayılan değer false'tur. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Çıktı öğelerinin optimize edilip edilmediğini gösterir. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Eğer OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu geçersiz olacaktır ve pagesetup'ın diğer ayarları hâlâ etkili olacaktır.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Eğer bu özellik true ise, bir Area çıkacaktır ve ölçek etkili olmayacaktır.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Yazdırılacak bir şey olmadığında boş bir sayfa çıkartılıp çıkartılmayacağını gösterir.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Sayfa kaydetme sürecinin ilerlemesini kontrol eder/gösterir.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Oluşturulan görüntüler için piksel formatını alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Hangi sayfaların yazdırılmayacağını gösterir.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Eğer PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu olacaktır. aksi takdirde böyle bir iletişim kutusu gösterilmez.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Sayfaları `Jpeg` formatında kaydederken uygulanacak oluşturulan görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar. Varsayılan değer 100'dür.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Çıktı dosya formatı türünü alır veya ayarlar. Tiff/XPS desteklenir(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../sheetset/visible/).(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Çizgilere, eğrilere ve doldurulmuş alanların kenarlarına yumuşatma (antialiasing) uygulanıp uygulanmayacağını belirtir. Varsayılan değer SmoothingMode.None'dur.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) SVG'deki css adının ön ekini alır ve ayarlar, varsayılan değer boş dizedir.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) Eğer bu özellik true ise, oluşturulan svg görünüm alanına sığacaktır.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda metin gösterim tipini alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Metin renderleme kalitesini belirtir. Varsayılan değer TextRenderingHint.SystemDefault'tir.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | [`ImageType`](../imageorprintoptions/imagetype/) Tiff ve [`TiffCompression`](../imageorprintoptions/tiffcompression/) Ccitt3 veya Ccitt4 olduğunda görüntüleri 1 bpp formata dönüştürürken kullanılan yöntemi alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | `Tiff` formatında sayfalar kaydedilirken uygulanacak bit derinliğini alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | `Tiff` formatında sayfalar kaydedilirken uygulanacak sıkıştırma türünü alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Oluşturulan görüntüler için dikey çözünürlüğü, inç başına nokta olarak alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) Görüntünün istenen genişlik ve yüksekliğini ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Görüntünün istenen genişlik ve yüksekliğini ayarlar.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek verileri doldurun
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Sütun grafik oluşturun
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // SVG görüntü seçeneklerini başlatın
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // SVG renderleme seçeneklerini yapılandırın
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Yazdırma kalitesini ve çözünürlüğü ayarlayın
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Grafiği yapılandırılmış seçeneklerle SVG'ye renderlayın
            chart.ToImage("chart_output.svg", svgOptions);

            // Çalışma kitabı kaydetme entegrasyonunu gösterin
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


