---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

يشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false

```csharp
public bool IsIECompatible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين خاصية IsIECompatible
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // حفظ دفتر العمل مع خيارات HTML
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


