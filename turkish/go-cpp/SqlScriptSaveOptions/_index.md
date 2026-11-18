---
title: "SqlScriptSaveOptions Sınıfı"
linktitle: "SqlScriptSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SqlScriptSaveOptions sınıfı. Go'da sqlscriptsaveoptions'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

SQL kaydetme seçeneklerini temsil eder.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | SQL dosyasını kaydetmek için seçenekler oluşturur. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | Oluşturmadan önce tablo adının var olup olmadığını kontrol eder |
| [SetCheckIfTableExists](./setcheckiftableexists/) | Oluşturmadan önce tablo adının var olup olmadığını kontrol eder |
| [GetColumnTypeMap](./getcolumntypemap/) | Farklı veritabanları için sütun tip haritasını alır ve ayarlar. |
| [SetColumnTypeMap](./setcolumntypemap/) | Farklı veritabanları için sütun tip haritasını alır ve ayarlar. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Sütunların veri tipini bulmak için tüm verileri kontrol eder. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Sütunların veri tipini bulmak için tüm verileri kontrol eder. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Her veri arasına boş satır ekler. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Her veri arasına boş satır ekler. |
| [GetSeparator](./getseparator/) | SQL betiğinin karakter ayırıcıyı alır ve ayarlar. |
| [SetSeparator](./setseparator/) | SQL betiğinin karakter ayırıcıyı alır ve ayarlar. |
| [GetOperatorType](./getoperatortype/) | SQL'in operatör tipini alır ve ayarlar. |
| [SetOperatorType](./setoperatortype/) | SQL'in operatör tipini alır ve ayarlar. |
| [GetPrimaryKey](./getprimarykey/) | Veri tablosunda hangi sütunun birincil anahtar olduğunu temsil eder. |
| [SetPrimaryKey](./setprimarykey/) | Veri tablosunda hangi sütunun birincil anahtar olduğunu temsil eder. |
| [GetCreateTable](./getcreatetable/) | Tablo oluşturma SQL'inin dışa aktarılıp aktarılmayacağını gösterir. |
| [SetCreateTable](./setcreatetable/) | Tablo oluşturma SQL'inin dışa aktarılıp aktarılmayacağını gösterir. |
| [GetIdName](./getidname/) | ID sütununun adını alır ve ayarlar. |
| [SetIdName](./setidname/) | ID sütununun adını alır ve ayarlar. |
| [GetStartId](./getstartid/) | Başlangıç kimliğini alır ve ayarlar. |
| [SetStartId](./setstartid/) | Başlangıç kimliğini alır ve ayarlar. |
| [GetTableName](./gettablename/) | Tablo adını alır ve ayarlar. |
| [SetTableName](./settablename/) | Tablo adını alır ve ayarlar. |
| [GetExportAsString](./getexportasstring/) | Tüm verilerin string değer olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [SetExportAsString](./setexportasstring/) | Tüm verilerin string değer olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [GetSheetIndexes](./getsheetindexes/) | Dışa aktarılan sayfaların indekslerini temsil eder. |
| [SetSheetIndexes](./setsheetindexes/) | Dışa aktarılan sayfaların indekslerini temsil eder. |
| [GetExportArea](./getexportarea/) | Dışa aktarma aralığını alır veya ayarlar. |
| [SetExportArea](./setexportarea/) | Dışa aktarma aralığını alır veya ayarlar. |
| [GetHasHeaderRow](./gethasheaderrow/) | Aralığın başlık satırı içerip içermediğini gösterir. |
| [SetHasHeaderRow](./sethasheaderrow/) | Aralığın başlık satırı içerip içermediğini gösterir. |
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
