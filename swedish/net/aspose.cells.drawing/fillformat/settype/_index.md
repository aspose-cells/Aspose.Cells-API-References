---
title: "FillFormat.SetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar den angivna fyllningsformatstypen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/settype/
---
## FillFormat.SetType property

Hämtar den angivna fyllningsformatstypen.

```csharp
[Obsolete("Use FillFormat.FillType instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FormatSetType SetType { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället FillFormat.FillType-egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* enum [FormatSetType](../../formatsettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


