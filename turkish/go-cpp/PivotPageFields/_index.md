---
title: "PivotPageFields Sınıfı"
linktitle: "PivotPageFields"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotPageFields sınıfı. Go'da pivotpagefields'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotpagefields/
---

## PivotPageFields class

Pivot tablo veri kaynağı konsolidasyon aralıklarıysa pivot sayfa öğelerini temsil eder. En fazla 4 öğe içerebilir.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Pivot sayfa alanı öğelerini temsil eder. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [AddPageField](./addpagefield/) | Bir sayfa alanı ekler. |
| [GetPageFieldCount](./getpagefieldcount/) | Sayfa alanı sayısını alır. |
| [AddIdentify](./addidentify/) | Her sayfa alanındaki hangi öğe etiketinin veri aralığını tanımlamak için kullanılacağını ayarlar. pageItemIndex.Length, PageFieldCount'e eşit olmalıdır, bu yüzden lütfen önce sayfa alanını ekleyin. |
