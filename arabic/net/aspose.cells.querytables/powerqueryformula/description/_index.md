---
title: "PowerQueryFormula.Description"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormula. يحصل على الوصف ويضبطه لصيغة Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

يحصل على وصف صيغة استعلام Power Query ويضبطه.

```csharp
public string Description { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // تحميل ملف موجود يحتوي على صيغ Power Query
                workbook = new Workbook("example.xlsx");

                // الوصول إلى صيغ Power Query الموجودة
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // عرض قيمة الوصف الحالية
                    Console.WriteLine("Current Description: " + formula.Description);

                    // تعيين وصف جديد
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // احفظ المصنف
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


