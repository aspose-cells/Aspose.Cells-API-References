---
title: "Font.IsNormalizeHeights"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. تشير إلى ما إذا كان سيتم تطبيق تطبيع الارتفاع على مقطع النص"
type: docs
url: /ar/net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

يشير إلى ما إذا كان سيتم تطبيق تطبيع الارتفاع على مجموعة النص.

```csharp
[Obsolete("Use TextOptions.IsNormalizeHeights property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsNormalizeHeights { get; set; }
```

### ملاحظات

فقط لخطوط الأشكال أو المخططات. ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [`IsNormalizeHeights`](../../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/). سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsNormalizeHeightsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            Font font = style.Font;

            // تعيين خاصية IsNormalizeHeights
            font.IsNormalizeHeights = true;
            Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Test Text");

            // تحقق من الخاصية
            Font cellFont = cell.GetStyle().Font;
            Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);

            // تعديل الخاصية
            cellFont.IsNormalizeHeights = false;
            Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


