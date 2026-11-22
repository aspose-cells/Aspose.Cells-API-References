---
title: "SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تعيين الفاصل للعناصر في صفوف البيانات بالمصفوفات في الصيغة"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray method

يضبط الفاصل للعناصر في بيانات صف المصفوفة في الصيغة.

```csharp
public void SetColumnSeparatorOfFormulaArray(char c)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| c | محرف | الفاصل المحدد |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            
            try
            {
                globalizationSettings.SetColumnSeparatorOfFormulaArray('|');
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                worksheet.Cells["A1"].SetArrayFormula("{1|2|3}", 1, 3);
                Console.WriteLine("Column separator for formula arrays set to '|'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetColumnSeparatorOfFormulaArray: {ex.Message}");
            }

            workbook.Save("SetColumnSeparatorOfFormulaArrayWithCharDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


