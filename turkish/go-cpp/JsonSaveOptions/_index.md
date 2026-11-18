---
title: "JsonSaveOptions Class"
linktitle: "JsonSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "JsonSaveOptions class. Go'da jsonsaveoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Çalışma kitabını JSON dosyası olarak kaydetme seçeneklerini temsil eder.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | JSON dosyasını kaydetmek için seçenekler oluşturur. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetExportStylePool](./getexportstylepool/) | Stilleri toplu olarak mı yoksa her hücreye ayrı ayrı mı dışa aktarılacağını belirtir. |
| [SetExportStylePool](./setexportstylepool/) | Stilleri toplu olarak mı yoksa her hücreye ayrı ayrı mı dışa aktarılacağını belirtir. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | JSON'a köprü (hyperlink) dışa aktarma türünü temsil eder. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | JSON'a köprü (hyperlink) dışa aktarma türünü temsil eder. |
| [GetSkipEmptyRows](./getskipemptyrows/) | Boş satırların atlanıp atlanmayacağını belirtir. |
| [SetSkipEmptyRows](./setskipemptyrows/) | Boş satırların atlanıp atlanmayacağını belirtir. |
| [GetSheetIndexes](./getsheetindexes/) | Dışa aktarılan sayfaların indekslerini temsil eder. |
| [SetSheetIndexes](./setsheetindexes/) | Dışa aktarılan sayfaların indekslerini temsil eder. |
| [GetSchemas](./getschemas/) | Her çalışma sayfasının orijinal JSON şeması. |
| [SetSchemas](./setschemas/) | Her çalışma sayfasının orijinal JSON şeması. |
| [GetExportArea](./getexportarea/) | Dışa aktarma aralığını alır veya ayarlar. |
| [SetExportArea](./setexportarea/) | Dışa aktarma aralığını alır veya ayarlar. |
| [GetHasHeaderRow](./gethasheaderrow/) | Aralığın başlık satırı içerip içermediğini gösterir. |
| [SetHasHeaderRow](./sethasheaderrow/) | Aralığın başlık satırı içerip içermediğini gösterir. |
| [GetExportAsString](./getexportasstring/) | Hücrelerin metin değerlerini JSON'a dışa aktarır. |
| [SetExportAsString](./setexportasstring/) | Hücrelerin metin değerlerini JSON'a dışa aktarır. |
| [GetIndent](./getindent/) | Girintiyi belirtir. |
| [SetIndent](./setindent/) | Girintiyi belirtir. |
| [GetExportNestedStructure](./getexportnestedstructure/) | Üst-alt hiyerarşi JSON yapısı olarak dışa aktarılır. |
| [SetExportNestedStructure](./setexportnestedstructure/) | Üst-alt hiyerarşi JSON yapısı olarak dışa aktarılır. |
| [GetExportEmptyCells](./getexportemptycells/) | Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını belirtir. |
| [SetExportEmptyCells](./setexportemptycells/) | Boş hücrelerin null olarak dışa aktarılıp aktarılmayacağını belirtir. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Dosyada yalnızca bir çalışma sayfası olsa bile Excel'i her zaman nesne olarak JSON'a dışa aktarılıp aktarılmayacağını belirtir. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Dosyada yalnızca bir çalışma sayfası olsa bile Excel'i her zaman nesne olarak JSON'a dışa aktarılıp aktarılmayacağını belirtir. |
| [GetToExcelStruct](./gettoexcelstruct/) | Excel dosyasının json yapısına dönüştürülüp dönüştürülmediğini gösterir. |
| [SetToExcelStruct](./settoexcelstruct/) | Excel dosyasının json yapısına dönüştürülüp dönüştürülmediğini gösterir. |
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
