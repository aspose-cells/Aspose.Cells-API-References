---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل ويضبط الدقة الافتراضية للصورة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

يحصل ويعيّن الدقة الافتراضية للصورة.

```csharp
public int DefaultImageResolution { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // ضبط الدقة الافتراضية للصورة
            workbook.Settings.DefaultImageResolution = 300;
            
            // إضافة ورقة عمل وإدراج صورة
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // التحقق من الدقة الافتراضية للصورة
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


