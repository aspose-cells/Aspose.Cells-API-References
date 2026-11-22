---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaParseOptions. تعريف لتحليل الدوال المخصصة"
type: docs
url: /ar/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

تعريف لتحليل الدوال المخصصة.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### ملاحظات

لبعض المتطلبات الخاصة، مثل حساب دالة مخصصة في محرك المستخدم المخصص، تحتاج بعض معلماتها إلى حسابها في وضع المصفوفة، يمكن باستخدام هذه الخاصية وضع علامة على تلك المعلمات كأنها في وضع المصفوفة عند تحليل الصيغة. وإلا سيتعين على المستخدم تحديث تلك الدوال المخصصة لاحقًا عبر [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) للحصول على النتيجة نفسها.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تعريف دالة مخصصة
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // إعداد خيارات تحليل الصيغة مع الدالة المخصصة
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // تعيين بيانات عينة
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // استخدام الدالة المخصصة في الصيغة
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // حساب دفتر العمل لتوضيح معالجة الدالة المخصصة
            workbook.CalculateFormula();

            // حفظ النتيجة
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


