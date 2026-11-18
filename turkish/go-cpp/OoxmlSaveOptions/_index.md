---
title: "OoxmlSaveOptions Sınıfı"
linktitle: "OoxmlSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "OoxmlSaveOptions sınıfı. Go'da ooxmlsaveoptions nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Office Open XML dosyasını kaydetme seçeneklerini temsil eder.

```go

type OoxmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewOoxmlSaveOptions](./newooxmlsaveoptions/) | Office Open XML dosyasını kaydetmek için seçenekleri oluşturur. |
| [NewOoxmlSaveOptions_SaveFormat](./newooxmlsaveoptions_saveformat/) | Office Open XML dosyasını kaydetmek için seçenekleri oluşturur. |
| [NewOoxmlSaveOptions_SaveOptions](./newooxmlsaveoptions_saveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetAsFlatOpc](./getasflatopc/) | Open XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmediğini gösterir. |
| [SetAsFlatOpc](./setasflatopc/) | Open XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmediğini gösterir. |
| [GetExportCellName](./getexportcellname/) | Excel2007 .xlsx (.xlsm, .xltx, .xltm) dosyasına hücre adının dışa aktarılıp aktarılmayacağını gösterir. Çıktı dosyasına SQL Server DTS tarafından erişilebilecekse, bu değer true olmalıdır. Değeri false olarak ayarlamak, büyük dosya oluştururken performansı önemli ölçüde artıracak ve dosya boyutunu azaltacaktır. Varsayılan değer true'tir. |
| [SetExportCellName](./setexportcellname/) | Excel2007 .xlsx (.xlsm, .xltx, .xltm) dosyasına hücre adının dışa aktarılıp aktarılmayacağını gösterir. Çıktı dosyasına SQL Server DTS tarafından erişilebilecekse, bu değer true olmalıdır. Değeri false olarak ayarlamak, büyük dosya oluştururken performansı önemli ölçüde artıracak ve dosya boyutunu azaltacaktır. Varsayılan değer true'tir. |
| [GetUpdateZoom](./getupdatezoom/) | Dosya kaydedilmeden önce ölçekleme faktörünün güncellenip güncellenmeyeceğini gösterir; eğer PageSetup.FitToPagesWide ve PageSetup.FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol ediyorsa. |
| [SetUpdateZoom](./setupdatezoom/) | Dosya kaydedilmeden önce ölçekleme faktörünün güncellenip güncellenmeyeceğini gösterir; eğer PageSetup.FitToPagesWide ve PageSetup.FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol ediyorsa. |
| [GetEnableZip64](./getenablezip64/) | Gerekli olduğunda zip arşivleri yazılırken ZIP64 uzantılarını kullan. |
| [SetEnableZip64](./setenablezip64/) | Gerekli olduğunda zip arşivleri yazılırken ZIP64 uzantılarını kullan. |
| [GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | OleObject'in Ooxml dosyalarının gömülüp gömülmeyeceğini gösterir. |
| [SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | OleObject'in Ooxml dosyalarının gömülüp gömülmeyeceğini gösterir. |
| [GetCompressionType](./getcompressiontype/) | ooxml dosyası için sıkıştırma türünü alır ve ayarlar. |
| [SetCompressionType](./setcompressiontype/) | ooxml dosyası için sıkıştırma türünü alır ve ayarlar. |
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
