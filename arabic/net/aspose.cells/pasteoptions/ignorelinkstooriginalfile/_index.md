---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. تجاهل الروابط إلى الملف الأصلي"
type: docs
url: /ar/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

تجاهل الروابط إلى الملف الأصلي.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // إنشاء بيانات عينة بصيغ قد ترتبط بالملف الأصلي
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // إنشاء ورقة عمل الوجهة والنطاق
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // تكوين خيارات اللصق لتجاهل الروابط إلى الملف الأصلي
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // نسخ مع خيارات اللصق المحددة
            dstRange.Copy(srcRange, pasteOptions);

            // احفظ المصنف
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


