---
title: "PageSetup.PrinterSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تحصل على إعدادات الطابعة الافتراضية وتضبطها"
type: docs
url: /ar/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

يحصل على إعدادات الطابعة الافتراضية ويضبطها.

```csharp
public byte[] PrinterSettings { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // الوصول إلى إعداد الصفحة
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين إعدادات الطابعة (كمصفوفة بايتات)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // تحقق من ضبط إعدادات الطابعة
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // احفظ المصنف
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


