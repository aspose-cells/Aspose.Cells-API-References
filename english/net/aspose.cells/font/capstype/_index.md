---
title: Font.CapsType
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the text caps type
type: docs
url: /net/aspose.cells/font/capstype/
---
## Font.CapsType property

Gets and sets the text caps type.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Remarks

Only for the fonts of Shapes or Charts. NOTE: This member is now obsolete. Instead, please use [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

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

### See Also

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


