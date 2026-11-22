---
title: "FormatCondition.SetFormula1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "FormatCondition method. يحدد القيمة أو التعبير المرتبط بهذا الشرط التنسيقي"
type: docs
url: /ar/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا سيتم اعتبارها قيمة عادية (نص, رقم, منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\"=...\"" |
| isR1C1 | منطقي | ما إذا كانت الصيغة صيغة R1C1. |
| isLocal | منطقي | ما إذا كانت الصيغة مُنسقة محليًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إضافة نطاق تنسيق شرطي
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // الحصول على أول شرط تنسيق
            FormatCondition fc = fcc[0];

            try
            {
                // استدعاء SetFormula1 مع معلمات (String, Boolean, Boolean)
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // اعرض النتيجة
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


