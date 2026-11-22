---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookSettings. تعيين نوع اتجاه الطباعة للمصنف بأكمله"
type: docs
url: /ar/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

ضبط نوع اتجاه الطباعة لكامل دفتر العمل.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | نوع اتجاه الصفحة |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // تعيين اتجاه الصفحة إلى Portrait لجميع أوراق العمل
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // تحقق من أن الاتجاه تم تعيينه بشكل صحيح
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### انظر أيضًا

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


