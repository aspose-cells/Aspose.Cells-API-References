---
title: "الفئة FormulaParseOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FormulaParseOptions. يمثل الخيارات عند تحليل الصيغة"
type: docs
url: /ar/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

يمثل الخيارات عند تحليل الصيغة.

```csharp
public class FormulaParseOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | ما إذا كان يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للدالة المعرفة من قبل المستخدم دون رابط خارجي. القيمة الافتراضية هي true (إذا تطابقت الدالة المعرفة من قبل المستخدم مع إحدى الإضافات في الروابط الخارجية الموجودة، فسيتم اعتبارها الإضافة). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | تعريف لتحليل الدوال المخصصة. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | ما إذا كانت الصيغة مُنسقة حسب اللغة المحلية. القيمة الافتراضية هي false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | ما إذا كان يتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false، فستُحفظ سلسلة الصيغة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو يُطلب بيانات الصيغة المحللة من قبل عمليات أخرى مثل حساب الصيغ. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | ما إذا كانت الصيغة بنمط الإشارة R1C1. القيمة الافتراضية هي false. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // إضافة صيغة إلى خلية باستخدام الخيارات
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // احفظ المصنف
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


