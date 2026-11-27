---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Hämtar alla celler som innehåller inbäddad bild"
type: docs
url: /sv/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Hämtar alla celler som innehåller inbäddad bild.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Returvärde

Enumerator för att enumerera alla Cell-objekt som innehåller inbäddad bild

### Anmärkningar

Om det inte finns någon bild som är inställd som "Place in Cell" i detta kalkylblad, returneras null.

### Exempel

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en bild i kalkylbladet (detta kommer inte att räknas av GetCellsWithPlaceInCellPicture)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // Lägg till en inbäddad bild i cell B3 (detta kommer att räknas)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Ta bort den flytande bilden
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Hämta celler med inbäddade bilder
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Spara och ladda om för att verifiera beständighet
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Verifiera efter omladdning
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


