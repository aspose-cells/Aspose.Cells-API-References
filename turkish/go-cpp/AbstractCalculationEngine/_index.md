---
title: "AbstractCalculationEngine Sınıf"
linktitle: "AbstractCalculationEngine"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AbstractCalculationEngine sınıfı. Go'da abstractcalculationengine'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için kullanıcının özel hesaplama motorunu temsil eder.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | Şu anda değerlendirilmekte olan işlevi referans alan tüm formülün hesaplamasını atlar. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | Bu motorun bir hesaplama yaparken parametrenin gerçek metnine ihtiyacı olup olmadığını gösterir.Default değer yanlıştır. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | Bu motorun parametrenin dizi modunda hesaplanması gerekip gerekmediğini gösterir. Varsayılan değer yanlıştır.If CalculationData.GetParamValueInArrayMode(int, int, int) özel işlevler hesaplanırken gerekli ise ve kullanıcı bunların tanımını (Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) ile) güncellememişse, bu özellik true olarak ayarlanmalıdır. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Yerleşik motorlar tarafından desteklenen yerleşik işlevlerin bu uygulama tarafından kontrol edilip işlenip işlenmeyeceği. Varsayılan yanlıştır. |
| [ForceRecalculate](./forcerecalculate/) | Paylaşılan formüller hesaplanırken verilen işlevin her zaman yeniden hesaplanmasını zorunlu kılıp kılmayacağı. |
