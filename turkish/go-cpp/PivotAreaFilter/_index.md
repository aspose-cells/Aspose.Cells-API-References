---
title: "PivotAreaFilter Sınıfı"
linktitle: "PivotAreaFilter"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotAreaFilter sınıfı. Go'da pivotareafilter'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

<see cref="PivotTable"/> için <see cref="PivotArea"/> filtresini temsil eder.

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsSubtotalSet](./issubtotalset/) | Bu filtre için ayarlanan alt toplamın hangisi olduğunu alır. |
| [SetSubtotals](./setsubtotals/) | Filtre için alt toplam. |
| [GetFieldIndex](./getfieldindex/) | Bu filtrenin referans verdiği kaynak alanlardaki alanın dizinini alır. -2 değeri değerler alanını gösterir. |
| [GetSelected](./getselected/) | Bu alanın seçimi olup olmadığını gösterir. Yalnızca PivotTable Taslak görünümünde çalışır. |
| [SetSelected](./setselected/) | Bu alanın seçimi olup olmadığını gösterir. Yalnızca PivotTable Taslak görünümünde çalışır. |
