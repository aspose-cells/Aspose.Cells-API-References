---
title: "PivotGlobalizationSettings Sınıfı"
linktitle: "PivotGlobalizationSettings"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotGlobalizationSettings sınıfı. Go'da pivotglobalizationsettings'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Pivot tablolar için küreselleştirme ayarlarını temsil eder.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetTextOfTotal](./gettextoftotal/) | PivotTable'daki "Total" etiketinin metnini alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | PivotTable'daki "Grand Total" etiketinin metnini alır. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | PivotTable'daki "(Multiple Items)" etiketinin metnini alır. |
| [GetTextOfAll](./gettextofall/) | PivotTable'daki "(All)" etiketinin metnini alır. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Belirtilen korumalı ad için metni alır. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | PivotTable'daki "Column Labels" etiketinin metnini alır. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | PivotTable'daki "Row Labels" etiketinin metnini alır. |
| [GetTextOfEmptyData](./gettextofemptydata/) | PivotTable'daki "(blank)" etiketinin metnini alır. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | PivotTable'daki değer alanı alan başlığının metnini alır. |
| [GetShortTextOf12Months](./getshorttextof12months/) | 12 ayın tüm kısa biçimli dizesini alır. |
| [GetTextOf24Hours](./gettextof24hours/) | 24 saatin tüm yerel biçimli dizesini alır. Varsayılan değer 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM'dir. |
| [GetTextOfOr](./gettextofor/) | "or" ifadesinin tüm yerel biçimli dizesini alır. |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Pivot gün grubu için sayı biçimini alır. Yalnızca pivot alanı günlere göre gruplanırken kullanılır. Varsayılan değer "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | 4 Çeyrek'in yerel metnini alır. |
| [GetTextOf4Quarters](./gettextof4quarters/) | 4 Çeyrek'in yerel metnini alır. |
| [GetTextOfYears](./gettextofyears/) | "Years" ifadesinin yerel metnini alır. |
| [GetTextOfQuarters](./gettextofquarters/) | "Quarters" öğesinin yerel metnini al. |
| [GetTextOfMonths](./gettextofmonths/) | "Months" öğesinin yerel metnini alır. |
| [GetTextOfDays](./gettextofdays/) | "Days" öğesinin yerel metnini alır. |
| [GetTextOfHours](./gettextofhours/) | "Hours" öğesinin yerel metnini alır. |
| [GetTextOfMinutes](./gettextofminutes/) | "Minutes" öğesinin yerel metnini alır. |
| [GetTextOfSeconds](./gettextofseconds/) | "Seconds" öğesinin yerel metnini alır |
| [GetTextOfRange](./gettextofrange/) | "Range" öğesinin yerel metnini alır |
| [GetTextOfAllPeriods](./gettextofallperiods/) | "All Periods" öğesinin yerel metnini alır |
| [GetTextOfSubTotal](./gettextofsubtotal/) | PivotTable'daki PivotFieldSubtotalType türünün metnini alır. |
| [GetNameOfDataField](./getnameofdatafield/) | Veri pivot alanının görüntüleme adını alır. Varsayılan format "Sum Of Field"dır. |
