---
title: "Sınıf GridImageOrPrintOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions sınıfı. Çalışma sayfasını görüntülere render ederken, çalışma sayfasını yazdırırken veya grafiği görüntüye render ederken seçenekleri belirtmeye olanak tanır."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Çalışma sayfasını görüntülere oluştururken, çalışma sayfasını yazdırırken veya grafiği görüntüye oluştururken seçenekleri belirtmeye izin verir.

```csharp
public class GridImageOrPrintOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | GridImageOrPrintOptions yapısı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt genişliği geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf, görüntüde blok olarak görünebilirler. Bu değeri true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipini kullanarak bu karakterleri göstermeye çalışır. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir DefaultFont ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Svg içinde gömülü görüntünün dosya adını belirtin. Bu, "c:\\xpsEmbedded" gibi bir dizinle tam yol olmalıdır. |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Metafile formatını belirten bir EmfType alır veya ayarlar. Varsayılan değer EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Izgara çizgi tipini alır veya ayarlar. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Oluşturulan görüntüler için yatay çözünürlüğü (inç başına nokta) alır veya ayarlar. Emf formatı dışındaki görüntü oluşturma yöntemlerine uygulanır. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Oluşturulan görüntülerin formatını alır veya ayarlar. Varsayılan değer: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Çıktı öğelerinin optimize edilip edilmediğini gösterir. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. Sayfa ayarının kağıt boyutu geçersiz olacak ve sayfa ayarının diğer ayarları hâlâ geçerli olacaktır. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Bu özellik true ise, bir Alan çıktılanır ve ölçekleme etkili olmaz. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır veya ayarlar. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Oluşturulan görüntüler için piksel formatını alır veya ayarlar. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Hangi sayfaların yazdırılmayacağını gösterir. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir. Aksi takdirde böyle bir iletişim kutusu gösterilmez. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Sayfaları `Jpeg` formatında kaydederken uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar. Varsayılan değer 100. |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Düzleştirme (antialiasing) işleminin çizgilere, eğrilere ve doldurulmuş alanların kenarlarına uygulanıp uygulanmayacağını belirtir. Varsayılan değer SmoothingMode.None'dur. |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Bu özellik true ise, oluşturulan svg görüntüleme alanına sığar. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin tipini alır veya ayarlar. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Metin renderleme kalitesini belirtir. Varsayılan değer TextRenderingHint.SystemDefault'dur. |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Oluşturulan görüntüler için dikey çözünürlüğü (inç başına nokta) alır veya ayarlar. Emf formatı dışındaki görüntü oluşturma yöntemlerine uygulanır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Görüntünün istenen genişlik ve yüksekliğini ayarlar. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | Render edilecek sayfaları ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır. Sıfır tabanlı sayfa indeksleri. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


