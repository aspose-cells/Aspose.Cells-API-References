---
title: "PdfSaveOptions Sınıfı"
linktitle: "PdfSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PdfSaveOptions sınıfı. Go dilinde pdfsaveoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pdfsaveoptions/
---

## PdfSaveOptions class

Pdf dosyasını kaydetme seçeneklerini temsil eder.

```go

type PdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPdfSaveOptions](./newpdfsaveoptions/) | PDF dosyasını kaydetmek için seçenekleri oluşturur. |
| [NewPdfSaveOptions_PaginatedSaveOptions](./newpdfsaveoptions_paginatedsaveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetEmbedStandardWindowsFonts](./getembedstandardwindowsfonts/) | True, TrueType yazı tiplerini gömmek için. Yalnızca ASCII karakterleri 32-127 etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülür. PDF/A-1a, PDF/A-1b standardı için yazı tipleri her zaman gömülür. Varsayılan değer True'dur. |
| [SetEmbedStandardWindowsFonts](./setembedstandardwindowsfonts/) | True, TrueType yazı tiplerini gömmek için. Yalnızca ASCII karakterleri 32-127 etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülür. PDF/A-1a, PDF/A-1b standardı için yazı tipleri her zaman gömülür. Varsayılan değer True'dur. |
| [GetBookmark](./getbookmark/) | PdfBookmarkEntry</see> nesnesini alır ve ayarlar. |
| [SetBookmark](./setbookmark/) | PdfBookmarkEntry</see> nesnesini alır ve ayarlar. |
| [GetCompliance](./getcompliance/) | Çıktı belgeleri için PDF standartları uyumluluk seviyesini alır veya ayarlar. |
| [SetCompliance](./setcompliance/) | Çıktı belgeleri için PDF standartları uyumluluk seviyesini alır veya ayarlar. |
| [GetSecurityOptions](./getsecurityoptions/) | Güvenliğin xls2pdf sonucunda gerektiği durumlarda bu seçenekleri ayarlayın. |
| [SetSecurityOptions](./setsecurityoptions/) | Güvenliğin xls2pdf sonucunda gerektiği durumlarda bu seçenekleri ayarlayın. |
| [GetCalculateFormula](./getcalculateformula/) | PDF dosyasını kaydetmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [SetCalculateFormula](./setcalculateformula/) | PDF dosyasını kaydetmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [GetPdfCompression](./getpdfcompression/) | Sıkıştırma algoritmasını belirtir. |
| [SetPdfCompression](./setpdfcompression/) | Sıkıştırma algoritmasını belirtir. |
| [SetImageResample](./setimageresample/) | Yeniden örnekleme görüntülerinin istenen PPI (inç başına piksel) ve JPEG kalitesini ayarlar. Tüm görüntüler belirtilen kalite ayarıyla JPEG'e dönüştürülecek ve belirtilen PPI'dan (inç başına piksel) büyük olan görüntüler yeniden örneklenir. |
| [GetCreatedTime](./getcreatedtime/) | PDF belgesinin oluşturulma zamanını alır ve ayarlar. |
| [SetCreatedTime](./setcreatedtime/) | PDF belgesinin oluşturulma zamanını alır ve ayarlar. |
| [GetProducer](./getproducer/) | Oluşturulan PDF belgesinin üreticisini alır ve ayarlar. |
| [SetProducer](./setproducer/) | Oluşturulan PDF belgesinin üreticisini alır ve ayarlar. |
| [GetOptimizationType](./getoptimizationtype/) | PDF optimizasyon tipini alır ve ayarlar. |
| [SetOptimizationType](./setoptimizationtype/) | PDF optimizasyon tipini alır ve ayarlar. |
| [GetCustomPropertiesExport](./getcustompropertiesexport/) | CustomDocumentPropertyCollection'ın PDF dosyasına nasıl dışa aktarılacağını belirleyen değeri alır veya ayarlar. Varsayılan değer None'dur. |
| [SetCustomPropertiesExport](./setcustompropertiesexport/) | CustomDocumentPropertyCollection'ın PDF dosyasına nasıl dışa aktarılacağını belirleyen değeri alır veya ayarlar. Varsayılan değer None'dur. |
| [GetExportDocumentStructure](./getexportdocumentstructure/) | Belge yapısının dışa aktarılıp aktarılmayacağını gösterir. |
| [SetExportDocumentStructure](./setexportdocumentstructure/) | Belge yapısının dışa aktarılıp aktarılmayacağını gösterir. |
| [GetDisplayDocTitle](./getdisplaydoctitle/) | Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini gösterir. |
| [SetDisplayDocTitle](./setdisplaydoctitle/) | Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini gösterir. |
| [GetFontEncoding](./getfontencoding/) | PDF içinde gömülü yazı tipi kodlamasını alır veya ayarlar. |
| [SetFontEncoding](./setfontencoding/) | PDF içinde gömülü yazı tipi kodlamasını alır veya ayarlar. |
| [GetWatermark](./getwatermark/) | Çıktıya filigranı alır veya ayarlar. |
| [SetWatermark](./setwatermark/) | Çıktıya filigranı alır veya ayarlar. |
| [GetEmbedAttachments](./getembedattachments/) | Excel'de Ole nesneleri için ekin gömülüp gömülmeyeceğini gösterir. |
| [SetEmbedAttachments](./setembedattachments/) | Excel'de Ole nesneleri için ekin gömülüp gömülmeyeceğini gösterir. |
| [GetZoomBehavior](./getzoombehavior/) | Oluşturulan PDF belgesi açıldığında ilk görüntüleme modunu alır veya ayarlar. Varsayılan değer PdfZoomBehavior.None. |
| [SetZoomBehavior](./setzoombehavior/) | Oluşturulan PDF belgesi açıldığında ilk görüntüleme modunu alır veya ayarlar. Varsayılan değer PdfZoomBehavior.None. |
| [GetZoomFactor](./getzoomfactor/) | Zoom yüzdesini alır veya ayarlar; whenZoomBehavior PdfZoomBehavior.ZoomFactor olduğunda. |
| [SetZoomFactor](./setzoomfactor/) | Zoom yüzdesini alır veya ayarlar; whenZoomBehavior PdfZoomBehavior.ZoomFactor olduğunda. |
| [GetDefaultFont](./getdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. MingLiu veya MS Gothic gibi bir DefaultFont ayarlayarak bu karakterlerin gösterilmesini sağlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır. |
| [SetDefaultFont](./setdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. MingLiu veya MS Gothic gibi bir DefaultFont ayarlayarak bu karakterlerin gösterilmesini sağlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. Bu özelliği true olarak ayarlayarak önce çalışma kitabının varsayılan yazı tipini kullanıp bu karakterleri göstermeyi deneyin. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. Bu özelliği true olarak ayarlayarak önce çalışma kitabının varsayılan yazı tipini kullanıp bu karakterleri göstermeyi deneyin. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Hücre yazı tipi karakterle uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Hücre yazı tipi karakterle uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. |
| [GetOnePagePerSheet](./getonepagepersheet/) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [SetOnePagePerSheet](./setonepagepersheet/) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu genişliği göz ardı edilir ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu genişliği göz ardı edilir ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [GetIgnoreError](./getignoreerror/) | Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik renderleme vb. hatalar olabilir. |
| [SetIgnoreError](./setignoreerror/) | Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik renderleme vb. hatalar olabilir. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktılanıp çıktılanmayacağını gösterir. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktılanıp çıktılanmayacağını gösterir. |
| [SetPageIndex](./setpageindex/) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar. |
| [GetPageIndex](./getpageindex/) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar. |
| [SetPageCount](./setpagecount/) | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [GetPageCount](./getpagecount/) | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [GetPrintingPageType](./getprintingpagetype/) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [SetPrintingPageType](./setprintingpagetype/) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [GetGridlineType](./getgridlinetype/) | Kılavuz çizgi tipini alır veya ayarlar. |
| [SetGridlineType](./setgridlinetype/) | Kılavuz çizgi tipini alır veya ayarlar. |
| [GetGridlineColor](./getgridlinecolor/) | Kılavuz çizgi rengini alır veya ayarlar. |
| [SetGridlineColor](./setgridlinecolor/) | Kılavuz çizgi rengini alır veya ayarlar. |
| [GetTextCrossType](./gettextcrosstype/) | Metin genişliği hücre genişliğinden büyük olduğunda gösterilen metin tipini alır veya ayarlar. |
| [SetTextCrossType](./settextcrosstype/) | Metin genişliği hücre genişliğinden büyük olduğunda gösterilen metin tipini alır veya ayarlar. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Varsayılan düzenleme dilini alır veya ayarlar. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Varsayılan düzenleme dilini alır veya ayarlar. |
| [GetSheetSet](./getsheetset/) | Renderlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Renderlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Render ederken DrawObject ve Bound'ı elde etmek için bu arayüzü uygular. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Render ederken DrawObject ve Bound'ı elde etmek için bu arayüzü uygular. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Emf meta dosyasını renderleme ayarı. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Emf meta dosyasını renderleme ayarı. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Renderleme sırasında özel ayarları alır veya ayarlar. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Renderleme sırasında özel ayarları alır veya ayarlar. |
| [GetRenderingBehavior](./getrenderingbehavior/) | Uygulanacak Excel'e özgü renderleme davranışlarını alır veya ayarlar. |
| [SetRenderingBehavior](./setrenderingbehavior/) | Uygulanacak Excel'e özgü renderleme davranışlarını alır veya ayarlar. |
| [GetSaveFormat](./getsaveformat/) | Kaydetme dosya formatını alır. |
| [GetClearData](./getcleardata/) | Dosya kaydedildikten sonra çalışma kitabını boş bırak. |
| [SetClearData](./setcleardata/) | Dosya kaydedildikten sonra çalışma kitabını boş bırak. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [GetMergeAreas](./getmergeareas/) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [SetMergeAreas](./setmergeareas/) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [GetCreateDirectory](./getcreatedirectory/) | Doğruysa ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [SetCreateDirectory](./setcreatedirectory/) | Doğruysa ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [GetSortNames](./getsortnames/) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [SetSortNames](./setsortnames/) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [GetSortExternalNames](./getsortexternalnames/) | Dosya kaydedilmeden önce dış tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [SetSortExternalNames](./setsortexternalnames/) | Dosya kaydedilmeden önce dış tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Kaydedilirken .xls dosyası olarak belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer true'dur. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Kaydedilirken .xls dosyası olarak belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer true'dur. |
