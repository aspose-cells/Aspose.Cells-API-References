---
title: "Font.CapsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. تحصل وتعيّن نوع الحروف الكبيرة للنص"
type: docs
url: /ar/net/aspose.cells/font/capstype/
---
## Font.CapsType property

تحصل وتعيّن نوع الحروف الكبيرة للنص.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### ملاحظات

فقط لخطوط الأشكال أو المخططات. ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/). سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCapsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("sample text");

            Style style = cell.GetStyle();
            style.Font.CapsType = TextCapsType.All;
            cell.SetStyle(style);

            workbook.Save("FontCapsTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


