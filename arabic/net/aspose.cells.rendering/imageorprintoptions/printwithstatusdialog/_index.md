---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. إذا كان PrintWithStatusDialog  true  سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // تهيئة دفتر عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // تعيين خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // إنشاء SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // طباعة إلى PDF
            sheetRender.ToImage(0, "output.png");

            // انتظر إنشاء الملف (منطق انتظار مبسط)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


