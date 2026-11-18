---
title: "LowCodeSaveOptionsProviderOfPlaceHolders Sınıfı"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "LowCodeSaveOptionsProviderOfPlaceHolders sınıfı. Go'da lowcodesaveoptionsproviderofplaceholders nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun yer tutucularla tanımlandığı kaydetme seçeneklerini sağlamak için uygulama.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Belirtilen şablonlara göre kaydetme seçenekleri sağlamak için bir örnek oluşturur. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.SheetIndex) arasındaki sayfa indeksi ofseti. |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.SheetIndex) arasındaki sayfa indeksi ofseti. |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.PartIndex) arasındaki bölünmüş parça indeksi ofseti. |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.PartIndex) arasındaki bölünmüş parça indeksi ofseti. |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Dosya yoluna her zaman sayfa indeksi veya adı eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi ve adı ve ilgili önek (SheetNamePrefix) dosya yoluna eklenmez. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Dosya yoluna her zaman sayfa indeksi veya adı eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi ve adı ve ilgili önek (SheetNamePrefix) dosya yoluna eklenmez. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Dosya yoluna her zaman bölünmüş parça indeksi eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek (SplitPartPrefix) dosya yoluna eklenmez. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Dosya yoluna her zaman bölünmüş parça indeksi eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek (SplitPartPrefix) dosya yoluna eklenmez. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | Çalışma sayfası indeksinin ön eki. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | Çalışma sayfası indeksinin ön eki. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | Çalışma sayfası indeksinin ön eki. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | Çalışma sayfası indeksinin ön eki. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Bölünmüş parça indeksinin ön eki. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Bölünmüş parça indeksinin ön eki. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | GetSaveOptions(SplitPartInfo) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | GetSaveOptions(SplitPartInfo) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [GetSaveOptions](./getsaveoptions/) | Şu anda bölünmüş parça için çıktı ayarlarını almak üzere kaydetme seçeneklerini alır. |
| [Finish](./finish/) | Mevcut bölünmüş parçayı işledikten sonra kaynakları serbest bırakır. |
