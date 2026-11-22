---
title: "WorkbookSettings.MaxRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل على أقصى فهرس صف يبدأ من الصفر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

يحصل على أقصى فهرس للصف، يبدأ من الصفر.

```csharp
public int MaxRow { get; }
```

### ملاحظات

إرجاع 65535 إذا كان تنسيق الملف هو Excel97-2003؛

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إظهار خاصية MaxRow
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // حاول الوصول إلى خلية تتجاوز MaxRow (يجب أن يرمي استثناءً)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // إنشاء منطقة خلايا باستخدام MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


