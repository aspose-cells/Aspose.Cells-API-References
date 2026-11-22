---
title: "FormulaParseOptions.Parse"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaParseOptions. ما إذا كان سيتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false فستظل سلسلة الصيغة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو تُطلب بيانات الصيغة المحللة في عمليات أخرى مثل حساب الصيغ."
type: docs
url: /ar/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

ما إذا كان يتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false، فستُحفظ سلسلة الصيغة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو يُطلب بيانات الصيغة المحللة من قبل عمليات أخرى مثل حساب الصيغ.

```csharp
public bool Parse { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // تعيين صيغ مع Parse=false (لن يتم تحليل الصيغ فورًا)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // حساب الصيغ (سيتم التحليل الآن)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


