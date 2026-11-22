---
title: "الفئة PowerQueryFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.QueryTables.PowerQueryFormula. تمثل تعريف صيغة استعلام Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

يمثل تعريف صيغة Power Query.

```csharp
public class PowerQueryFormula
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | يحصل على وصف صيغة استعلام Power Query ويضبطه. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | يحصل على تعريف صيغة استعلام Power Query. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | يحصل على اسم المجموعة التي تحتوي على صيغة استعلام Power Query هذه. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | يحصل على اسم صيغة استعلام Power Query ويضبطه. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | يحصل على جميع عناصر صيغة استعلام Power Query. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | يحصل على نوع صيغة استعلام Power Query هذه. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // الوصول إلى مجموعة PowerQueryFormulas من DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // تحقق مما إذا كان هناك أي صيغ موجودة
                if (formulas.Count > 0)
                {
                    // احصل على أول PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // عرض الخصائص للقراءة فقط
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // عرض وتعديل الخصائص القابلة للقراءة والكتابة
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // عرض عدد عناصر الصيغة
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // احفظ المصنف
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormula: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


