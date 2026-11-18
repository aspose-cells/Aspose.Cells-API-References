---
title: "OfdSaveOptions Sınıfı"
linktitle: "OfdSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "OfdSaveOptions sınıfı. Go'da ofdsaveoptions'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/ofdsaveoptions/
---

## OfdSaveOptions class

OFD (Açık Sabit Düzen Belgesi) dosyasını kaydetme seçeneklerini temsil eder.

```go

type OfdSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewOfdSaveOptions](./newofdsaveoptions/) | OFD dosyasını kaydetmek için seçenekleri oluşturur. |
| [NewOfdSaveOptions_PaginatedSaveOptions](./newofdsaveoptions_paginatedsaveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
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
