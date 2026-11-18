---
title: "PivotItem Sınıfı"
linktitle: "PivotItem"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotItem sınıfı. Go'da pivotitem'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotitem/
---

## PivotItem class

Bir PivotField raporundaki bir öğeyi temsil eder.

```go

type PivotItem struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsHidden](./ishidden/) | Pivot öğesinin gizli olup olmadığını alır ve ayarlar. |
| [SetIsHidden](./setishidden/) | Pivot öğesinin gizli olup olmadığını alır ve ayarlar. |
| [GetPosition](./getposition/) | Bu öğenin alandaki tüm PivotItem'lar içindeki indeksini belirtir. |
| [SetPosition](./setposition/) | Bu öğenin alandaki tüm PivotItem'lar içindeki indeksini belirtir. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | Aynı üst düğüm altındaki PivotItem'larda konum indeksini belirtir. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | Aynı üst düğüm altındaki PivotItem'larda konum indeksini belirtir. |
| [Move](./move/) | Öğeyi yukarı veya aşağı hareket ettirir |
| [IsDetailHidden](./isdetailhidden/) | Bu pivot öğesinin detayının gizli olup olmadığını alır ve ayarlar. |
| [SetIsDetailHidden](./setisdetailhidden/) | Bu pivot öğesinin detayının gizli olup olmadığını alır ve ayarlar. |
| [IsCalculatedItem](./iscalculateditem/) | Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir. |
| [GetFormula](./getformula/) | Bu hesaplanmış öğenin formülünü alır. Yalnızca öğe hesaplanmış bir öğe olduğunda çalışır. |
| [IsMissing](./ismissing/) | Öğenin veri kaynağından kaldırılıp kaldırılmadığını gösterir. |
| [GetStringValue](./getstringvalue/) | Pivot öğesinin string değerini alır. Değer null ise, "" döndürür. |
| [GetDoubleValue](./getdoublevalue/) | Pivot öğesinin double değerini alır. Değer null ya da sayı değilse, 0 döndürür. |
| [GetDateTimeValue](./getdatetimevalue/) | Pivot öğesinin tarih saat değerini alır. Değer null ise, DateTime.MinValue döndürür. |
| [GetValue](./getvalue/) | Pivot öğesinin değerini alır |
| [GetName](./getname/) | Pivot öğesinin adını alır. |
| [SetName](./setname/) | Pivot öğesinin adını alır. |
