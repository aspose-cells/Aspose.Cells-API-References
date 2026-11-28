---
title: "Sınıf PptxSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PptxSaveOptions sınıfı. pptx kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/pptxsaveoptions/
---
## PptxSaveOptions class

pptx kaydetme seçeneklerini temsil eder.

```csharp
public class PptxSaveOptions : PaginatedSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PptxSaveOptions](pptxsaveoptions/#constructor)() | pptx kaydetme seçeneklerini temsil eder. |
| [PptxSaveOptions](pptxsaveoptions/#constructor_1)(bool) | .pptx dosyasını kaydetme seçeneklerini temsil eder. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AdjustFontSizeForRowType](../../aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/) { get; set; } | Satır yüksekliği küçük olduğunda yazı tipi boyutunun ayarlanması gereken çizgi tipini temsil eder. |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu genişliği yok sayılacak ve pagesetup'ın diğer ayarları hâlâ geçerli olacaktır.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [AsFlatOpc](../../aspose.cells/pptxsaveoptions/asflatopc/) { get; set; } | Open XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmediğini gösterir |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceği gösterir.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bunu true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipini bu karakterleri göstermek için kullanmaya çalışır.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dosya kaydedildikten sonra çalışma kitabını boş bırak. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Renderleme sırasında özel ayarları alır veya ayarlar.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Varsayılan düzenleme dilini alır veya ayarlar.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Renderleme sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedXlsxAsChartDataSource](../../aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/) { get; set; } | Grafiğin veri kaynağı olarak bir xlsx dosyasının gömülüp gömülmediğini gösterir. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Emf metafilesi renderleme ayarı.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer doğrudur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ExportViewType](../../aspose.cells/pptxsaveoptions/exportviewtype/) { get; set; } | PowerPoint'e dışa aktarırken görüntüleme tipini alır ve ayarlar. Varsayılan dışa aktarma tipi yazdırma gibi çalışır. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Izgara çizgi rengini alır veya ayarlar.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Izgara çizgi tipini alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Render ederken hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik render'ı vb. hatalar olabilir. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreHiddenRows](../../aspose.cells/pptxsaveoptions/ignorehiddenrows/) { get; set; } | Excel'den PowerPoint'e dönüştürürken gizli satırların göz ardı edilip edilmeyeceğini gösterir. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Hücre yazı tipi bununla uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu geçersiz olur ve sayfa ayarının diğer ayarları hâlâ geçerli olur. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Yazdırılacak bir şey olmadığında boş bir sayfa çıktılanıp çıktılanmayacağını gösterir. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Sayfa kaydetme sürecinin ilerlemesini kontrol eder/gösterir. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Hangi sayfaların yazdırılmayacağını gösterir. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Uygulanacak Excel'e özgü render davranışlarını alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveAsEditableShapes](../../aspose.cells/pptxsaveoptions/saveaseditableshapes/) { get; set; } | Tüm çizim nesnelerini pptx dosyasında düzenlenebilir şekiller olarak kaydedin, böylece PowerPoint'te düzenleyebilirsiniz. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Kaydetme dosya formatını alır. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda gösterilecek metin tipini alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Uyarı geri aramasını alır veya ayarlar. ([`SaveOptions`](../saveoptions/) sınıfından devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using Aspose.Cells.Rendering;
    using System;

    public class PptxSaveOptionsDemo
    {
        public static void PptxSaveOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekleyin.
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // PptxSaveOptions bir örnek oluşturun
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                IgnoreHiddenRows = true,
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows,
                ExportViewType = SlideViewType.Print,
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = true,
                CheckFontCompatibility = true,
                IsFontSubstitutionCharGranularity = true,
                OnePagePerSheet = true,
                AllColumnsInOnePagePerSheet = true,
                IgnoreError = true,
                OutputBlankPageWhenNothingToPrint = true,
                PageIndex = 0,
                PageCount = 1,
                PrintingPageType = PrintingPageType.IgnoreBlank,
                GridlineType = GridlineType.Dotted,
                TextCrossType = TextCrossType.CrossKeep,
                DefaultEditLanguage = DefaultEditLanguage.English,
                SheetSet = SheetSet.Visible,
                EmfRenderSetting = EmfRenderSetting.EmfOnly,
                ClearData = true,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = true
            };

            // Çalışma kitabını PPTX dosyası olarak kaydedin
            workbook.Save("PptxSaveOptionsExample.pptx", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


