---
title: "PivotArea Sınıfı"
linktitle: "PivotArea"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotArea sınıfı. Go'da pivotarea'yı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotarea/
---

## PivotArea class

Pivot tablonun seçili alanını sunar.

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | PivotTable'ın seçili alanını sunar. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetFilters](./getfilters/) | Bu PivotArea için tüm filtreleri alır. |
| [Select](./select/) | Filtreli alanı seç. |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Bölgede bir alanı alan olarak seç. |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Bölgede bir alanı alan olarak seç. |
| [GetOnlyData](./getonlydata/) | Bir öğe seçimi için yalnızca veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir. |
| [SetOnlyData](./setonlydata/) | Bir öğe seçimi için yalnızca veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir. |
| [GetOnlyLabel](./getonlylabel/) | Bir öğe seçimi için yalnızca veri etiketlerinin seçilip seçilmediğini gösterir. |
| [SetOnlyLabel](./setonlylabel/) | Bir öğe seçimi için yalnızca veri etiketlerinin seçilip seçilmediğini gösterir. |
| [IsRowGrandIncluded](./isrowgrandincluded/) | Satır toplamının dahil edilip edilmediğini gösterir. |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | Satır toplamının dahil edilip edilmediğini gösterir. |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | Sütun toplamının dahil edilip edilmediğini gösterir. |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Sütun toplamının dahil edilip edilmediğini gösterir. |
| [GetAxisType](./getaxistype/) | Bu kuralın uygulandığı PivotTable bölgesini alır ve ayarlar. |
| [SetAxisType](./setaxistype/) | Bu kuralın uygulandığı PivotTable bölgesini alır ve ayarlar. |
| [GetRuleType](./getruletype/) | Seçim kuralının türünü alır ve ayarlar. |
| [SetRuleType](./setruletype/) | Seçim kuralının türünü alır ve ayarlar. |
| [IsOutline](./isoutline/) | Kuralın taslak modunda olan bir alana başvurup başvurmadığını gösterir. |
| [SetIsOutline](./setisoutline/) | Kuralın taslak modunda olan bir alana başvurup başvurmadığını gösterir. |
| [GetCellAreas](./getcellareas/) | Bu pivot alanının hücre alanlarını alır. |
