---
title: "الفئة CustomFunctionDefinition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.CustomFunctionDefinition. تعريف الدالة المخصصة للحساب باستخدام محرك المستخدم المخصص"
type: docs
url: /ar/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

تعريف الدالة المخصصة للحساب باستخدام محرك المستخدم المخصص.

```csharp
public class CustomFunctionDefinition
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | يحصل على مؤشرات معلمات الدالة المخصصة المعطاة التي تحتاج إلى حسابها في وضع المصفوفة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء نسخة جديدة من CustomFunctionDefinition
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // إنشاء نسخة جديدة من FormulaParseOptions وتعيين CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // إضافة ورقة عمل إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // تعريف صيغة مخصصة
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // تحليل الصيغة المخصصة باستخدام FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // احفظ المصنف
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


