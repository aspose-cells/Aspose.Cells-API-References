---
title: "الفئة PowerQueryFormulaItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.QueryTables.PowerQueryFormulaItem. تمثل عنصر صيغة استعلام Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

يمثل عنصر صيغة Power Query.

```csharp
public class PowerQueryFormulaItem
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | يحصل على نوع هذا العنصر (دالة، معلمة، قائمة، ثابت، أو غير معروف). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | يحصل على اسم العنصر. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | يحصل على القيمة النصية للعنصر. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | يحصل على قيمة العنصر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مصنف جديد (يمكن أن يكون ملفًا موجودًا إذا كان لديك بيانات Power Query)
                Workbook workbook = new Workbook();

                // الوصول إلى كائن DataMashup الذي يحتوي على صيغ PowerQuery
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // التكرار عبر جميع صيغ PowerQuery وعناصرها
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // عرض خاصية الاسم للقراءة فقط
                        Console.WriteLine($"Item Name: {item.Name}");

                        // عرض خاصية القيمة للقراءة والكتابة
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


