---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان يتم فحص تنسيق الرقم المخصص عند تعيين Style.Custom"
type: docs
url: /ar/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // أولاً قم بتعيين تنسيق رقم مخصص صالح
            style.Custom = "#,##0.00";
            
            // تمكين الفحص الصارم
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // حاول تعيين تنسيق رقم مخصص غير صالح
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


