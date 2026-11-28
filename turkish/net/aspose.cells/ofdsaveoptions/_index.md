---
title: "OfdSaveOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.OfdSaveOptions sınıfı. OFDOpen Fixedlayout Belge dosyasını kaydetmek için seçenekleri temsil eder"
type: docs
url: /tr/net/aspose.cells/ofdsaveoptions/
---
## OfdSaveOptions class

OFD (Open Fixed-layout Document) dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class OfdSaveOptions : PaginatedSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OfdSaveOptions](ofdsaveoptions/)() | OFD dosyasını kaydetmek için seçenekleri oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu genişliği yok sayılacak ve pagesetup'ın diğer ayarları hâlâ geçerli olacaktır.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
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
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Emf metafilesi renderleme ayarı.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer doğrudur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Izgara çizgi rengini alır veya ayarlar.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Izgara çizgi tipini alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Render ederken hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik render'ı vb. hatalar olabilir. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
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
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Kaydetme dosya formatını alır. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda gösterilecek metin tipini alır veya ayarlar. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Uyarı geri aramasını alır veya ayarlar. ([`SaveOptions`](../saveoptions/) sınıfından devralınmıştır.) |

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


