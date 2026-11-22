---
title: "FormatCondition.SetFormula2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "FormatCondition method. يحدد القيمة أو التعبير المرتبط بهذا الشرط التنسيقي"
type: docs
url: /ar/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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

            // إضافة شرط تنسيق
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // الحصول على أول شرط تنسيق
            FormatCondition fc = fcs[0];

            try
            {
                // استدعِ SetFormula2 مع المعلمات (String, Boolean, Boolean)
                fc.SetFormula2("25", false, false);

                // اعرض النتيجة
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // طبق بعض الأنماط لجعل التأثير مرئيًا
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


