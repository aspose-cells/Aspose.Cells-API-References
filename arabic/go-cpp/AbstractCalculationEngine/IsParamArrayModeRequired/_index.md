---
title: "طريقة IsParamArrayModeRequired"
linktitle: "IsParamArrayModeRequired"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "طريقة IsParamArrayModeRequired. تغلف الدالة التي تمثل isparamarraymoderequired في Go."
type: docs
weight: 200
url: /ar/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

يشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. القيمة الافتراضية هي false. إذا كان مطلوبًا استدعاء CalculationData.GetParamValueInArrayMode(int, int, int) عند حساب الدوال المخصصة ولم يقم المستخدم بتحديث التعريف لها (عن طريق Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition))، يجب ضبط هذه الخاصية إلى true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## ملاحظات


## انظر أيضًا

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
