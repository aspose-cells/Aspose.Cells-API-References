---
title: "WorkbookSettings.BuildVersion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحدد الإصدار العام المتدرج للتطبيق"
type: docs
url: /ar/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

يحدد الإصدار العام المتزايد للتطبيق.

```csharp
public string BuildVersion { get; set; }
```

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // ضبط الإعدادات الأساسية
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // عرض خاصية BuildVersion
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // احفظ المصنف
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


