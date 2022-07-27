---
title: ImageOrPrintOptions
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma sayfasını görüntülere dönüştürürken çalışma sayfasını yazdırırken veya tabloyu görüntüye dönüştürürken seçenekleri belirlemeye izin verir.
type: docs
weight: 5140
url: /tr/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Çalışma sayfasını görüntülere dönüştürürken, çalışma sayfasını yazdırırken veya tabloyu görüntüye dönüştürürken seçenekleri belirlemeye izin verir.

```csharp
public class ImageOrPrintOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuç olarak yalnızca bir sayfaya çıkar. Sayfa kurulumunun kağıt boyutunun genişliği geçersiz olacak ve diğer sayfa kurulumu ayarları etkili olmaya devam edecek. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında, pdf'de blok olarak görünebilirler,image. Bu karakterleri önce göstermek için çalışma kitabının varsayılan yazı tipini kullanmayı denemek için bunu true olarak ayarlayın. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | İstemci, bu EventHandler kullanılarak her sayfayı yazdırırken yazıcıya özel çıktı verebilir |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | İstemci, bu EventHandler kullanarak her sayfayı yazdırırken yazıcının sayfa ayarını kontrol edebilir. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Varsayılan düzenleme dilini alır veya ayarlar. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında, pdf,image. 'de blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmadıysa, Aspose.Cells bu unicode karakterleri göstermek için sistem varsayılan yazı tipini kullanır. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Oluştururken DrawObject ve Bound almak için bu arabirimi uygular. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | svg'deki gömülü görüntünün dosya adını belirtin. Bu, "c:\\xpsEmbedded" gibi bir dizine sahip tam yol olmalıdır |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Metafile.. biçimini belirten bir EmfType alır veya ayarlarVarsayılan değer EmfPlusDual'dır. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Kılavuz çizgisi türünü alır veya ayarlar. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Oluşturulan görüntüler için inç başına nokta cinsinden yatay çözünürlüğü alır veya ayarlar. Emf biçimindeki görüntüler dışında görüntü oluşturma yöntemini uygular. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Oluşturulan görüntülerin biçimini alır veya ayarlar. varsayılan değer: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Hücrelerin genişlik ve yüksekliğinin hücre değerine göre otomatik olarak uydurulup uydurulmadığını gösterir. Varsayılan değer false'tur. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Hücre yazı tipi uyumlu olmadığında yalnızca karakter yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Çıktı öğelerinin optimize edilip edilmeyeceğini belirtir. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuç olarak yalnızca bir sayfaya çıkar. Sayfa kurulumunun kağıt boyutu geçersiz olacak ve diğer sayfa kurulumu ayarları etkili olmaya devam edecek. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Bu özellik true ise, bir Alan çıktısı alınır ve hiçbir ölçek etkili olmaz. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Yazdırılacak hiçbir şey olmadığında boş bir sayfanın çıktısının alınıp alınmayacağını belirtir. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Kaydedilecek sayfaların sayısını alır veya ayarlar. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Sayfa kaydetme işleminin ilerlemesini kontrol edin/gösterin. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Oluşturulan görüntüler için piksel biçimini alır veya ayarlar. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Hangi sayfaların yazdırılmayacağını belirtir. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | PrintWithStatusDialog = true ise, geçerli yazdırma durumunu gösteren bir iletişim kutusu olacaktır. yoksa böyle bir iletişim kutusu gösterilmeyecektir. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Oluşturulan görüntülerin kalitesini belirleyen bir değer alır veya ayarlar yalnızca sayfaları`JPEG` biçim. Varsayılan değer 100 'dir |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Çıktı dosyası biçimini alır veya ayarlar type Destek Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Çizgilere, eğrilere ve doldurulmuş alanların kenarlarına yumuşatma (antialiasing) uygulanıp uygulanmayacağını belirtir. Varsayılan değer SmoothingMode'dur.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | bu özellik doğruysa, oluşturulan svg bağlantı noktasını görüntülemek için uygun olacaktır. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda metin türünü görüntüleyen alır veya ayarlar. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Metin işleme kalitesini belirtir. Varsayılan değer, TextRenderingHint.SystemDefault 'dir. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Yalnızca sayfaları dosyaya kaydederken uygulanacak bit derinliğini alır veya ayarlar.`tiftik` biçim. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Yalnızca sayfaları dosyaya kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar.`tiftik` biçim. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Oluşturulan görüntünün arka planının şeffaf olması gerekip gerekmediğini gösterir. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Oluşturulan görüntülerin dikey çözünürlüğünü inç başına nokta olarak alır veya ayarlar. Emf biçimindeki görüntü dışında görüntü oluşturma yöntemini uygular. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Uyarı geri aramasını alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Görüntünün istenen genişliğini ve yüksekliğini ayarlar. |

### Örnekler

```csharp

[C#]

//Görüntü veya Yazdırma Seçeneklerini Ayarla
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Çıktı görüntü biçimini ayarla
options.ImageType = ImageType.Png;

// Yatay çözünürlüğü ayarla
options.HorizontalResolution = 300;

// Dikey Çözünürlüğü Ayarla
options.VerticalResolution = 300;

//Çalışma Kitabını Hazırla
Workbook book = new Workbook("test.xls");

//ImageOrPrint Seçeneklerini kullanarak grafiği Resim olarak kaydet
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Görüntü veya Yazdırma Seçeneklerini Ayarlayın
Dim options As New ImageOrPrintOptions()

'Çıktı görüntü biçimini ayarla
options.ImageType = ImageType.Png

'Yatay çözünürlüğü ayarla
options.HorizontalResolution = 300

'Dikey Çözünürlüğü Ayarla
options.VerticalResolution = 300

'Örnek Çalışma Kitabı
Dim book As New Workbook("test.xls")

'ImageOrPrint Seçeneklerini kullanarak grafiği Görüntü olarak kaydedin
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
