---
title: "LoadFilter Sınıfı"
linktitle: "LoadFilter"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "LoadFilter sınıfı. Go'da loadfilter'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/loadfilter/
---

## LoadFilter class

Şablondan çalışma kitabı yüklenirken veri yükleme seçenekleri sağlayan filtreyi temsil eder.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | Varsayılan filtre seçenekleri LoadDataFilterOptions::All ile bir LoadFilter oluşturur. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Verilen filtre seçenekleriyle bir LoadFilter oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Yüklenmesi gereken veriyi belirten filtre seçeneklerini alır. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Yüklenmesi gereken veriyi belirten filtre seçeneklerini ayarlar. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Yüklenmesi gereken sayfaları (indeksleri) ve sıralamayı belirtir. Varsayılan değer null'dır; bu, şablon dosyasındaki tüm sayfaların varsayılan sırayla yüklenmesi anlamına gelir. Null değilse ve bazı sayfa indeksleri dönen dizide yoksa, o sayfa yüklenmez. |
| [StartSheet](./startsheet/) | Verilen çalışma sayfası yüklenmeden önce filtre seçeneklerini hazırlar. Kullanıcının LoadFilter uygulaması, bu çalışma sayfası için verilerin nasıl yükleneceğini belirten LoadDataFilterOptions'ı değiştirebilir. |
