---
title: "PasteOptions.Transpose"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. True لنقل الصفوف والأعمدة عند لصق النطاق. القيمة الافتراضية هي False"
type: docs
url: /ar/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True لعكس الصفوف والأعمدة عند لصق النطاق. القيمة الافتراضية هي False.

```csharp
public bool Transpose { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نمط المصدر وتطبيقه على النطاق الأفقي
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // إنشاء خيارات اللصق مع النقل
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // نسخ مع النقل إلى النطاق العمودي
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // احفظ المصنف
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


