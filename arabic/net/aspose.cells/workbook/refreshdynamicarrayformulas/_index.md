---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تقوم بتحديث صيغ المصفوفة الديناميكية لتنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية. الصيغ الأخرى في المصنف لن تُحسب بشكل متكرر حتى إذا تم استخدامها بواسطة صيغ المصفوفة الديناميكية"
type: docs
url: /ar/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) لن يتم حساب الصيغ الأخرى في المصنف بشكل متكرر حتى إذا تم استخدامها بواسطة صيغ المصفوفة الديناميكية.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| حساب | منطقي | ما إذا كان يحسب ويحدّث قيم الخلايا لتلك صيغ المصفوفة الديناميكية |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // إعداد البيانات الأولية وصيغ المصفوفة الديناميكية
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // تغيير النطاق وتحديث الصيغ
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية)

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| حساب | منطقي | ما إذا كان يحسب ويحدّث قيم الخلايا لتلك صيغ المصفوفة الديناميكية |
| copts | CalculationOptions | الخيارات لحساب الصيغ |

### ملاحظات

لأسباب تتعلق بالأداء، لا نقوم بتحديث جميع صيغ المصفوفة الديناميكية تلقائيًا عندما تتغير الصيغة نفسها أو البيانات التي تشير إليها. لذلك يحتاج المستخدم إلى استدعاء هذه الطريقة يدويًا بعد تلك العمليات التي قد تؤثر على صيغ المصفوفة الديناميكية، مثل استيراد/تعيين قيم الخلايا، إدراج/حذف الصفوف/الأعمدة/النطاقات، ... إلخ. بالنسبة لمعظم الصيغ التي تحتوي على دوال، يتطلب حساب نطاق الانسكاب أيضًا حساب الصيغة، لذا يُفضَّل عمومًا استخدام القيمة true لعلامة "calculate". إذا كانت الصيغة بسيطة، مثل إشارة إلى نطاق أو مصفوفة (على سبيل المثال "=C1:E5", "={1,2;3,4}", ...)، أو دالة بسيطة على نطاق أو مصفوفة (على سبيل المثال "=ABS(C1:E5)", "=1+{1,2;3,4}", ...)، وجميع الصيغ سيتم حسابها لاحقًا (مثلًا عبر [`CalculateFormula`](../calculateformula/))، فإن استخدام القيمة false لعلامة "calculate" قد يجنّب الحساب المكرر لتحسين الأداء.

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة صيغة مصفوفة ديناميكية نموذجية
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // إنشاء خيارات الحساب
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // تحديث صيغ المصفوفة الديناميكية مع خيارات الحساب
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // حساب صيغ المصنف
            workbook.CalculateFormula(opts);
            
            // إخراج النتيجة من A1:A5
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


