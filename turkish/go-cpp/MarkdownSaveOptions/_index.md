---
title: "MarkdownSaveOptions Sınıfı"
linktitle: "MarkdownSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "MarkdownSaveOptions sınıfı. Go'da markdownsaveoptions'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Markdown için kaydetme seçeneklerini temsil eder.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Markdown belgesini kaydetmek için seçenekler oluşturur |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetEncoding](./getencoding/) | Varsayılan kodlamayı alır ve ayarlar. |
| [SetEncoding](./setencoding/) | Varsayılan kodlamayı alır ve ayarlar. |
| [GetFormatStrategy](./getformatstrategy/) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini alır ve ayarlar. |
| [SetFormatStrategy](./setformatstrategy/) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini alır ve ayarlar. |
| [GetLineSeparator](./getlineseparator/) | Satır ayırıcıyı alır ve ayarlar. |
| [SetLineSeparator](./setlineseparator/) | Satır ayırıcıyı alır ve ayarlar. |
| [GetTableHeaderType](./gettableheadertype/) | Tablonun başlığının nasıl ayarlandığını alır ve ayarlar. |
| [SetTableHeaderType](./settableheadertype/) | Tablonun başlığının nasıl ayarlandığını alır ve ayarlar. |
| [GetSheetSet](./getsheetset/) | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Markdown'a Base64 formatında kaydedilen görüntülerin belirlenip belirlenmediğini belirtir.Varsayılan değer true'dur. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Markdown'a Base64 formatında kaydedilen görüntülerin belirlenip belirlenmediğini belirtir.Varsayılan değer true'dur. |
| [GetCalculateFormula](./getcalculateformula/) | Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [SetCalculateFormula](./setcalculateformula/) | Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Hipermetin bağlantısının satır içi biçim yerine referans tanımları kullanılarak dışa aktarılıp aktarılmayacağını gösterir.Varsayılan değer false'tur. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Hipermetin bağlantısının satır içi biçim yerine referans tanımları kullanılarak dışa aktarılıp aktarılmayacağını gösterir.Varsayılan değer false'tur. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir.Etkinleştirildiğinde, sütunlar belirtilen karakterle (genellikle boşluk için ' ') hücre içeriği doldurularak hizalanır.\0 olarak ayarlandığında sütun hizalaması devre dışı bırakılır (varsayılan). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir.Etkinleştirildiğinde, sütunlar belirtilen karakterle (genellikle boşluk için ' ') hücre içeriği doldurularak hizalanır.\0 olarak ayarlandığında sütun hizalaması devre dışı bırakılır (varsayılan). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir.Varsayılan değer false'tur. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir.Varsayılan değer false'tur. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | OfficeMath nesnelerinin Markdown'a nasıl dışa aktarılacağını gösterir, varsayılan değer Image'dır. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | OfficeMath nesnelerinin Markdown'a nasıl dışa aktarılacağını gösterir, varsayılan değer Image'dır. |
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
