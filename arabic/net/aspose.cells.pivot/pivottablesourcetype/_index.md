---
title: "تعداد PivotTableSourceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotTableSourceType enum. يمثل نوع مصدر البيانات لجدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

يمثل نوع مصدر البيانات لجدول pivot.

```csharp
public enum PivotTableSourceType : byte
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Sheet | `1` | يحدد أن بيانات المصدر هي نطاق. |
| External | `2` | يحدد أنه يتم استخدام بيانات مصدر خارجية. |
| Consolidation | `4` | يحدد أنه يتم استخدام نطاقات دمج متعددة كمصدر للبيانات. |
| Scenario | `8` | يتم تعبئة بيانات المصدر من بنية داخلية مؤقتة. |
| Unknown | `9` | مصدر بيانات غير معروف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بيانات عينة إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // إنشاء مجموعة جداول محورية
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // إضافة جدول محوري باستخدام Sheet كنمط المصدر
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // عرض نوع المصدر
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // عرض أنواع مصدر مختلفة
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // احفظ المصنف
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


