---
title: "FillFormat.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar och anger fyllningstypen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Hämtar och anger fyllningstypen.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
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

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Visa aktuellt Type-värde
            Console.WriteLine("Current Type value: " + fill.Type);

            // Ändra Type till Gradient (föråldrad egenskap som används för demonstration)
            fill.Type = FillType.Gradient;

            // Applicera tvåfärgsgradient-effekt
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Spara den modifierade arbetsboken
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


