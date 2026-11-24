---
title: "FillFormat.SetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Ruft den eingestellten FillFormat-Typ ab."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/settype/
---
## FillFormat.SetType property

Ruft den eingestellten FillFormat-Typ ab.

```csharp
[Obsolete("Use FillFormat.FillType instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FormatSetType SetType { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die FillFormat.FillType-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertySetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fillFormat = shape.Fill;

            Console.WriteLine("Current SetType value: " + fillFormat.SetType);

            fillFormat.SetType = FormatSetType.IsGradientSet;
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            Console.WriteLine("New SetType value: " + fillFormat.SetType);

            workbook.Save("FillFormatSetTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FormatSetType](../../formatsettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


