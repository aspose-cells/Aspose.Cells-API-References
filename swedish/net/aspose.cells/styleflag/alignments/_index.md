---
title: "StyleFlag.Alignments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Justeringsinställning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

Justeringinställning kommer att tillämpas.

```csharp
public bool Alignments { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Skapa ett stilobjekt och sätt justeringsegenskaper
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Skapa en stilflagga och aktivera justeringsegenskaper
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Applicera stilen på cellen med stilflaggan
            cell.SetStyle(style, styleFlag);

            // Visa de aktuella justeringsinställningarna
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Ändra stilflaggan för att inaktivera justeringsegenskaper
            styleFlag.Alignments = false;
            
            // Skapa en ny stil med annan justering
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Tillämpa den nya stilen – justeringar kommer inte att förändras eftersom flaggan är falsk
            cell.SetStyle(newStyle, styleFlag);

            // Visa de oförändrade justeringsinställningarna
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Spara arbetsboken
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


