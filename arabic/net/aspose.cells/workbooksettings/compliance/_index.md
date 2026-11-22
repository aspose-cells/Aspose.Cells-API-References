---
title: "WorkbookSettings.Compliance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحدد نسخة OOXML للمستند الناتج. القيمة الافتراضية هي Ecma376_2006"
type: docs
url: /ar/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

يحدد إصدار OOXML للمستند الناتج. القيمة الافتراضية هي Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### ملاحظات

فقط لملفات .xlsx.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyComplianceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorkbookSettings settings = workbook.Settings;
            
            // تعيين الامتثال إلى الوضع الصارم
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


