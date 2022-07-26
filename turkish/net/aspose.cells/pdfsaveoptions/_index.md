---
title: PdfSaveOptions
second_title: Aspose.Cells for .NET API Referansı
description: Pdf dosyasını kaydetme seçeneklerini temsil eder.
type: docs
weight: 4500
url: /tr/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Pdf dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class PdfSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Pdf dosyasını kaydetme seçeneklerini oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuç olarak yalnızca bir sayfaya çıkar. Sayfa kurulumunun kağıt boyutunun genişliği yok sayılacak ve diğer sayfa kurulumu ayarları etkili olmaya devam edecek. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Alır ve ayarlar[`PdfYer İşaretiGirişi`](../../aspose.cells.rendering/pdfbookmarkentry) nesne. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Pdf dosyasını kaydetmeden önce formüllerin hesaplanıp hesaplanmayacağını belirtir. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Metindeki her karakter için yazı tipi uyumluluğunun kontrol edilip edilmeyeceğini belirtir. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında, pdf'de blok olarak görünebilirler,image. Bu karakterleri önce göstermek için çalışma kitabının varsayılan yazı tipini kullanmayı denemek için bunu true olarak ayarlayın. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Dosyayı kaydettikten sonra çalışma kitabını boşaltın. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | Çalışma kitabı, bu özellikte PdfCompliance'a göre pdf'ye dönüştürülür. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Doğruysa ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Pdf belgesinin oluşturulma zamanını alır ve ayarlar. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Yolu belirleyen bir değer alır veya ayarlar[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) PDF dosyasına aktarılır. Varsayılan değer Yok'tur. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Varsayılan düzenleme dilini alır veya ayarlar. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında, pdf,image. 'de blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmadıysa, Aspose.Cells bu unicode karakterleri göstermek için sistem varsayılan yazı tipini kullanır. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Pencerenin başlık çubuğunun belge başlığını gösterip göstermediğini gösterir. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Oluştururken DrawObject ve Bound almak için bu arabirimi uygular. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True type yazı tiplerini gömmek için True. Yalnızca 32-127 ASCII karakterlerini etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülüdür. PDF/A-1a, PDF/A-1b standardı için yazı tipleri her zaman gömülüdür. Varsayılan değer doğrudur. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Emf meta dosyası oluşturma ayarı. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Belge yapısının dışa aktarılıp aktarılmayacağını belirtir. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | pdf'de gömülü yazı tipi kodlamasını alır veya ayarlar. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Kılavuz çizgisi türünü alır veya ayarlar. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Oluştururken hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, resim, grafik oluşturma vb. hata olabilir. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Hücre yazı tipi uyumlu olmadığında yalnızca karakter yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuç olarak yalnızca bir sayfaya çıkar. Sayfa kurulumunun kağıt boyutu geçersiz olacak ve diğer sayfa kurulumu ayarları etkili olmaya devam edecek. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | pdf optimizasyon türünü alır ve ayarlar. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Yazdırılacak hiçbir şey olmadığında boş bir sayfanın çıktısının alınıp alınmayacağını belirtir. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Kaydedilecek sayfaların sayısını alır veya ayarlar. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Sayfa kaydetme işleminin ilerlemesini kontrol edin/gösterin. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Sıkıştırma algoritmasını belirtin |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Hangi sayfaların yazdırılmayacağını belirtir. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Oluşturulan pdf belgesinin üreticisini alır ve ayarlar. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Grafik önbelleği verilerinin yenilenip yenilenmediğini gösterir |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Kayıt dosyası biçimini alır. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Dosyayı kaydetmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Dosyayı kaydetmeden önce tanımlanmış adların sıralanıp sıralanmayacağını gösterir. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Metin genişliği hücre genişliğinden büyük olduğunda metin türünü görüntüleyen alır veya ayarlar. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmediğini gösterir. Varsayılan değer false'tur. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Uyarı geri aramasını alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Yeniden örnek görüntülerin ve jpeg kalitesinin istenen ÜFE'sini (inç başına piksel) ayarlar. Tüm resimler, belirtilen kalite ayarıyla JPEG'e dönüştürülecek, ve belirtilen ÜFE'den (inç başına piksel) daha büyük olan resimler yeniden örneklenecek. |

### Ayrıca bakınız

* class [SaveOptions](../saveoptions)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
