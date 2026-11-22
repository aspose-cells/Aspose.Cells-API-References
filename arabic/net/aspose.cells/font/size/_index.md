---
title: "Font.Size"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. تحصل أو تعيّن حجم الخط"
type: docs
url: /ar/net/aspose.cells/font/size/
---
## Font.Size property

يحصل على أو يضبط حجم الخط.

```csharp
public int Size { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين نص بأحجام خطوط مختلفة
            Cell cell1 = worksheet.Cells["A1"];
            cell1.Value = "Text with size 12";
            Style style1 = workbook.CreateStyle();
            style1.Font.Size = 12;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A3"];
            cell2.Value = "Text with size 16";
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 16;
            cell2.SetStyle(style2);

            // احفظ المصنف
            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


