---
title: "TxtSaveOptions Sınıfı"
linktitle: "TxtSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "TxtSaveOptions sınıfı. Go'da txtsaveoptions nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

CSV/sekme ayrılmış/diğer metin formatı için kaydetme seçeneklerini temsil eder.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Metin dosyası kaydetme seçeneklerini oluşturur. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Metin dosyası kaydetme seçeneklerini oluşturur. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetSeparator](./getseparator/) | Metin dosyasının karakter sınırlayıcısını alır ve ayarlar. |
| [SetSeparator](./setseparator/) | Metin dosyasının karakter sınırlayıcısını alır ve ayarlar. |
| [GetSeparatorString](./getseparatorstring/) | Ayırıcı olarak bir dize değerini alır ve ayarlar. |
| [SetSeparatorString](./setseparatorstring/) | Ayırıcı olarak bir dize değerini alır ve ayarlar. |
| [GetEncoding](./getencoding/) | Varsayılan kodlamayı alır ve ayarlar. |
| [SetEncoding](./setencoding/) | Varsayılan kodlamayı alır ve ayarlar. |
| [GetQuoteType](./getquotetype/) | Dışa aktarılan metin dosyasında değerlerin nasıl tırnak içine alınacağını alır veya ayarlar. |
| [SetQuoteType](./setquotetype/) | Dışa aktarılan metin dosyasında değerlerin nasıl tırnak içine alınacağını alır veya ayarlar. |
| [GetFormatStrategy](./getformatstrategy/) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini alır ve ayarlar. |
| [SetFormatStrategy](./setformatstrategy/) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini alır ve ayarlar. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | MS Excel'in yaptığı gibi, baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. Varsayılan değer true'tır. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | MS Excel'in yaptığı gibi, baştaki boş satır ve sütunların kırpılıp kırpılmayacağını gösterir. Varsayılan değer true'tır. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Bir satırdaki sondaki boş hücrelerin kırpılıp kırpılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. Varsayılan değer false olduğundan, boş satırın içeriği varsayılan olarak boş olacaktır. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Boş satır için ayırıcıların çıktılanıp çıktılanmayacağını gösterir. Varsayılan değer false olduğundan, boş satırın içeriği varsayılan olarak boş olacaktır. |
| [GetExportArea](./getexportarea/) | Dışa aktarılacak hücre aralığı. |
| [SetExportArea](./setexportarea/) | Dışa aktarılacak hücre aralığı. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Style.QuotePrefix true olduğunda, tek tırnak işaretinin bir hücrenin değeriyle birlikte dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Style.QuotePrefix true olduğunda, tek tırnak işaretinin bir hücrenin değeriyle birlikte dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetExportAllSheets](./getexportallsheets/) | Tüm sayfaların metin dosyasına dışa aktarılıp aktarılmayacağını gösterir. False ise, sadece aktif sayfa dışa aktarılır, tıpkı MS Excel gibi. |
| [SetExportAllSheets](./setexportallsheets/) | Tüm sayfaların metin dosyasına dışa aktarılıp aktarılmayacağını gösterir. False ise, sadece aktif sayfa dışa aktarılır, tıpkı MS Excel gibi. |
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
