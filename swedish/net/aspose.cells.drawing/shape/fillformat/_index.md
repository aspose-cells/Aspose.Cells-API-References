---
title: "Shape.FillFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Returnerar ett MsoFillFormat-objekt som innehåller fyllningsformateringsegenskaper för den angivna formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Returnerar ett MsoFillFormat-objekt som innehåller fyllningsformateringsegenskaper för den angivna formen.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Fill-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera FillFormat-egenskapen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // Få åtkomst till FillFormat-egenskapen (skrivskyddad)
                MsoFillFormat fillFormat = shape.FillFormat;

                // Visa aktuella FillFormat-egenskaper
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // Modifiera FillFormat-egenskaper (eftersom den inte är skrivskyddad)
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Visa uppdaterade FillFormat-egenskaper
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Spara arbetsboken
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


