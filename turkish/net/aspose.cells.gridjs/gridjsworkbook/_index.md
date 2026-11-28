---
title: "GridJsWorkbook sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.GridJsWorkbook sınıfı. GridJs için ana giriş sınıfını temsil eder."
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

GridJs için ana giriş sınıfını temsil eder

```csharp
public class GridJsWorkbook
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | GridJsWorkbook'ın yeni bir örneğini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Elektronik tablo dosyasını depolamak için önbellek dizinini alır/ayarlar. Bu ayarlanmamışsa, [`FileCacheDirectory`](../config/filecachedirectory/) veya [`CacheImp`](./cacheimp/) adresindeki statik özelliği kullanacağız. |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Çalışma kitabı ayarlarını temsil eder. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | İçe aktarma dosyası için uyarı geri çağrısını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Uygular (burns) çalışma kitabındaki tüm redaksiyon işlemlerini, redaksiyon şekillerini ve bunların hedef şekillerini kaldırarak ya da hedef hücre aralığı içeriğini temizleyerek. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol eder. Bu yöntem yalnızca İşbirlikçi mod için uygulanır. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Tüm JSON önbelleğini temizle |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | UID'ye göre JSON önbelleğini temizle (UpdateCell gibi yalnızca UID kullanılan senaryolar için) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Görseli veya şekli kopyalar. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Hata mesajı dizesini JSON formatında alır. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Bellek verisinden JSON dizesini alır, JSON içindeki varsayılan dosya adı: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Bellek verisinden JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Bellek verisinden JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Gömülü OLE nesnesinin bayt dizisi verisini alır. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | Belirtilen sayfanın JSON'unu (önbellekle birlikte) al. |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | Tam çalışma kitabının JSON'ını (önbellekle) al |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Excel dosyasını dosya yolundan içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Excel dosyasını Workbook nesnesinden içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Excel dosyasını yükleme formatı ile dosya akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Excel dosyasını dosya yolundan içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Excel dosyasını Workbook nesnesinden içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Excel dosyasını yükleme formatı ve açma şifresi ile dosya akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Excel dosyasını dosya akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Excel dosyasını dosya yolundan ve açma şifresiyle içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Excel dosyasını yükleme formatı ve açma şifresi ile dosya akışından içe aktarır. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Excel dosyasını JSON formatındaki dizeden içe aktarır. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Çalışma sayfasına dosya akışı veya URL'den (dosya akışı ya da URL sağlanmalıdır) görüntü ekler veya p.type AutoShapeType'tan biri olduğunda şekil ekler. |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Bellekteki Workbook'tan JSON oluşturur ve belirtilen akıma yazar. İsteğe bağlı olarak, oluşturulan JSON daha hızlı sonraki alımlar için önbelleğe alınır. JsonToStreamByUid ile temel farklar: - Bu yöntem mevcut bellek içi Workbook durumunu (wb alanı) kullanır - JsonToStreamByUid, Workbook'u disk üzerindeki .cells önbellek dosyalarından yeniden yükler - Değişikliklerden sonra mevcut çalışma kitabı durumunu dışa aktarmak istediğinizde bu yöntemi kullanın - Önceden önbelleğe alınmış bir dosya durumundan JSON yeniden oluşturmanız gerektiğinde JsonToStreamByUid'yi kullanın. Önbellekleme davranışı (uid sağlandığında): - Oluşturma öncesi JSON önbelleği kontrol eder (L1 bellek + L2 disk) - Önbellek yoksa, bellek içi workbook'tan JSON oluşturur - Oluşturulan JSON gelecekteki istekler için önbelleğe kaydedilir |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Belirtilen benzersiz kimliği kullanarak dosyanın JSON dizesini önbellekten al, JSON içinde çıktı dosya adını ayarla ve akıma yaz. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini alır. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten al ve akıma yaz. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Bellek verisine toplu bir güncelleme uygular. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Excel dosyası üzerinde JSON işlemleri dizisine dayalı redaksiyon gerçekleştirir. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Bellek verisini belirtilen dosya adıyla önbellek dosyasına kaydeder ve ayrıca açma şifresini ayarlar, kaydetme formatı dosya adının uzantısına dayanır. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Bellek verisini sream'e, orijinal dosya formatına dayanarak kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Bellek verisini dosya yoluna kaydeder, dosyanın uzantısı varsa, kaydetme formatı dosya uzantısına dayanır. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Bellek verisini sream'e kaydeder, kaydetme formatı html'dir. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Bellek verisini dosya yoluna kaydeder, kaydetme formatı html'dir. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Bellek verisini sream'e kaydeder, kaydetme formatı pdf'dir. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Bellek verisini dosya yoluna kaydeder, kaydetme formatı pdf'dir. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Bellek verisini sream'e kaydeder, kaydetme formatı xlsx'tir. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Bellek verisini dosya yoluna kaydeder, kaydetme formatı xlsx'tir. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Yükleme işlemi için InterruptMonitor ayarlar. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Kaydetme işlemi için InterruptMonitor ayarlar. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Çalışma kitabındaki redaksiyon şekillerinin saydamlığını ayarlar. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Çalışma sayfasındaki tüm dize değerlerini hedef dile çevir. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Güncelleme işlemini uygular. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Dosya uzantısına göre yükleme biçimini alır. |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Görselin akışını al. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Görselin URL'sini alır. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Verilen dosya adını kullanarak dosya önbelleği için yeni benzersiz bir kimlik oluşturur. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Denetleyiciden temel görüntü alma eylem URL'sini ayarlayın. |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Önbellek depolama için özel uygulama, önbelleği akış biçiminde depolamak istiyorsanız, bunu ayarlamanız ve uygulamanız gerekir. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Hesaplama motoru için özel uygulama, özel hesaplama yapmak istiyorsanız, bunu ayarlamanız ve uygulamanız gerekir. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | Görüntünün türü için sabit değer. |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Güncelleme işlemini izlemek için güncelleme izleyiciyi alır/ayarlar. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


