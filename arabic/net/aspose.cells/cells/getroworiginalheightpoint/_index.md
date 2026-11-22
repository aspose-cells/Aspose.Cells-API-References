---
title: "Cells.GetRowOriginalHeightPoint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على ارتفاع الصف الأصلي بوحدة النقطة إذا كان الصف مخفيًا"
type: docs
url: /ar/net/aspose.cells/cells/getroworiginalheightpoint/
---
## Cells.GetRowOriginalHeightPoint method

يحصل على ارتفاع الصف الأصلي بوحدة النقطة إذا كان الصف مخفيًا

```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetRowHeight(int,bool,CellsUnitType). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // احفظ الارتفاع الأصلي قبل التعديل
            double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
            
            // عدل ارتفاع الصف
            cells.SetRowHeight(0, 25.5);

            try
            {
                // احصل على الارتفاع الأصلي بعد التعديل
                double originalHeight = cells.GetRowOriginalHeightPoint(0);
                double currentHeight = cells.GetRowHeight(0);

                Console.WriteLine($"Original row height: {originalHeight} points");
                Console.WriteLine($"Current row height: {currentHeight} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
            }

            workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


