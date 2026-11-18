---
title: "LowCodeSaveOptionsProviderOfAssembling Sınıfı"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "LowCodeSaveOptionsProviderOfAssembling sınıfı. Go'da lowcodesaveoptionsproviderofassembling'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun şu şekilde adlandırıldığı (dizinler içerebilir) kaydetme seçeneklerini sağlamak için uygulama: <see cref="PathHeader"/>+<see cref="SheetPrefix"/>+SheetIndex (veya SheetName)+<see cref="SplitPartPrefix"/>+SplitPartIndex+<see cref="PathTail"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Varsayılan yapıcı. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetPathHeader](./getpathheader/) | Dosya yolunun başlık kısmı (sayfa ve bölünmüş parçanın eklenen içeriğinden önce). |
| [SetPathHeader](./setpathheader/) | Dosya yolunun başlık kısmı (sayfa ve bölünmüş parçanın eklenen içeriğinden önce). |
| [GetPathTail](./getpathtail/) | Dosya yolunun son kısmı (sıra numaralarından sonra). Dosya adı uzantısını içermelidir. |
| [SetPathTail](./setpathtail/) | Dosya yolunun son kısmı (sıra numaralarından sonra). Dosya adı uzantısını içermelidir. |
| [GetUseSheetName](./getusesheetname/) | Dosya yolunu sayfa adıyla, sayfa indeksi yerine oluşturup oluşturmayacağını belirler. Varsayılan değer false'tur. |
| [SetUseSheetName](./setusesheetname/) | Dosya yolunu sayfa adıyla, sayfa indeksi yerine oluşturup oluşturmayacağını belirler. Varsayılan değer false'tur. |
| [GetSheetPrefix](./getsheetprefix/) | Çalışma sayfası indeksinin ön eki. |
| [SetSheetPrefix](./setsheetprefix/) | Çalışma sayfası indeksinin ön eki. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Bölünmüş parça indeksinin ön eki. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Bölünmüş parça indeksinin ön eki. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.SheetIndex) arasındaki sayfa indeksi ofseti. |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.SheetIndex) arasındaki sayfa indeksi ofseti. |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.PartIndex) arasındaki bölünmüş parça indeksi ofseti. |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Dosya yolunda kullanılan ve gerçek değer (SplitPartInfo.PartIndex) arasındaki bölünmüş parça indeksi ofseti. |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Dosya yoluna her zaman sayfa indeksi veya adının eklenip eklenmeyeceğini belirler. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi (veya adı) ve ilgili ön ek dosya yoluna eklenmez. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Dosya yoluna her zaman sayfa indeksi veya adının eklenip eklenmeyeceğini belirler. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi (veya adı) ve ilgili ön ek dosya yoluna eklenmez. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Dosya yoluna her zaman bölünmüş parça indeksinin eklenip eklenmeyeceğini belirler. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili ön ek dosya yoluna eklenmez. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Dosya yoluna her zaman bölünmüş parça indeksinin eklenip eklenmeyeceğini belirler. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili ön ek dosya yoluna eklenmez. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | GetSaveOptions(SplitPartInfo) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | GetSaveOptions(SplitPartInfo) içinde kaydetme seçenekleri örneği oluşturmak için şablon. |
| [GetSaveOptions](./getsaveoptions/) | Şu anda bölünmüş parça için çıktı ayarlarını almak üzere kaydetme seçeneklerini alır. |
| [Finish](./finish/) | Mevcut bölünmüş parçayı işledikten sonra kaynakları serbest bırakır. |
