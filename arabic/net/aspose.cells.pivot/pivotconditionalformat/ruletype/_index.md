---
title: "PivotConditionalFormat.RuleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotConditionalFormat. احصل على نوع القاعدة واضبطه لتنسيق الشرط للجدول المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotconditionalformat/ruletype/
---
## PivotConditionalFormat.RuleType property

احصل على نوع القاعدة واضبطه لتنسيق الجدول المحوري الشرطي .

```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotConditionalFormatPropertyRuleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء بيانات قليلة للجدول المحوري
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "Value";

                // إنشاء جدول محوري
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // إضافة تنسيق شرطي
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];

                // عرض خاصية RuleType
                Console.WriteLine("Initial RuleType: " + format.RuleType);
                
                // ضبط نوع قاعدة جديد
                format.RuleType = PivotConditionFormatRuleType.Row;
                Console.WriteLine("Updated RuleType: " + format.RuleType);

                workbook.Save("RuleTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


