---
title: "XmlSaveOptions Sınıfı"
linktitle: "XmlSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "XmlSaveOptions sınıfı. Go'da xmlsaveoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

Çalışma kitabını XML dosyası olarak kaydetme seçeneklerini temsil eder.

```go

type XmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewXmlSaveOptions](./newxmlsaveoptions/) | XML dosyası kaydetmek için seçenekler oluşturur. |
| [NewXmlSaveOptions_SaveOptions](./newxmlsaveoptions_saveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetSheetIndexes](./getsheetindexes/) | Dışa aktarılan sayfaların indekslerini temsil eder. |
| [SetSheetIndexes](./setsheetindexes/) | Dışa aktarılan sayfaların indekslerini temsil eder. |
| [GetExportArea](./getexportarea/) | Dışa aktarma aralığını alır veya ayarlar. |
| [SetExportArea](./setexportarea/) | Dışa aktarma aralığını alır veya ayarlar. |
| [GetHasHeaderRow](./gethasheaderrow/) | Aralığın başlık satırı içerip içermediğini gösterir. |
| [SetHasHeaderRow](./sethasheaderrow/) | Aralığın başlık satırı içerip içermediğini gösterir. |
| [GetXmlMapName](./getxmlmapname/) | Dosyada XML haritası dışa aktarılıyor olup olmadığını gösterir. |
| [SetXmlMapName](./setxmlmapname/) | Dosyada XML haritası dışa aktarılıyor olup olmadığını gösterir. |
| [GetSheetNameAsElementName](./getsheetnameaselementname/) | Sayfanın adının öğenin adı olarak dışa aktarılıp aktarılmadığını gösterir. |
| [SetSheetNameAsElementName](./setsheetnameaselementname/) | Sayfanın adının öğenin adı olarak dışa aktarılıp aktarılmadığını gösterir. |
| [GetDataAsAttribute](./getdataasattribute/) | Elemanın öznitelikleri olarak veri dışa aktarımının yapılıp yapılmadığını gösterir. |
| [SetDataAsAttribute](./setdataasattribute/) | Elemanın öznitelikleri olarak veri dışa aktarımının yapılıp yapılmadığını gösterir. |
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
