---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ConditionalFormattingCollection. إزالة جميع التنسيقات الشرطية في النطاق"
type: docs
url: /ar/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

إزالة جميع التنسيقات الشرطية في النطاق.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | صف البداية للنطاق. |
| startColumn | Int32 | عمود البداية للنطاق. |
| totalRows | Int32 | عدد الصفوف في النطاق. |
| totalColumns | Int32 | عدد الأعمدة في النطاق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة التنسيق الشرطي
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // أضف بعض قواعد التنسيق الشرطي
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // استدعِ RemoveArea مع المعلمات (Int32, Int32, Int32, Int32)
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // تحقق من التأثير عن طريق فحص العدد (سيكون 0 إذا تمت إزالة جميع التنسيقات)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


