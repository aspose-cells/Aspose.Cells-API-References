---
title: "WorkbookSettings.WindowLeft"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة بوحدة النقطة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة، بوحدة النقطة.

```csharp
public double WindowLeft { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // عيّن خاصية WindowLeft لتحديد موضع النافذة 100 بكسل من اليسار
            settings.WindowLeft = 100;

            // عيّن خصائص نافذة أخرى للعرض
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // إضافة بيانات عينة إلى ورقة العمل
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // احفظ المصنف
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


