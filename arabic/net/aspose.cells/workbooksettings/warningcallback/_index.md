---
title: "WorkbookSettings.WarningCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل أو تعين رد النداء للتحذير"
type: docs
url: /ar/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

يحصل أو يضبط رد النداء التحذيري.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين رد الاتصال للتحذير
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // إنشاء ورقة عمل مع سيناريو تحذير محتمل (نطاق مسمى مكرر)
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // سيؤدي هذا إلى تشغيل تحذير حول الاسم المكرر
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // حفظ المصنف (سيؤدي إلى تشغيل رد النداء للتحذير)
            workbook.Save("WarningCallbackExample.xlsx");
        }
    }

    public class WarningCallbackImplementation : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.WarningType}, Description: {warningInfo.Description}");
        }
    }
}
```

### انظر أيضًا

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


