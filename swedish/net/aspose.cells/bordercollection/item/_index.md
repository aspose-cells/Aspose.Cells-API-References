---
title: "BorderCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BorderCollection egenskap. Hämtar Border-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Hämtar [`Border`](../../border/) elementet på det angivna indexet.

```csharp
public Border this[BorderType borderType] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| borderType | Den border som ska hämtas. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Hämta cellen och dess stil
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Åtkomst till BorderCollection från stilen
                BorderCollection borders = style.Borders;

                // Visa det aktuella värdet för Item-egenskapen (läsoperation)
                // Obs: Item-egenskapen är skrivskyddad och returnerar ett Border-objekt
                // Item-egenskapen kräver en BorderType-parameter
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Spara resultatet
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
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

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


