---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar en uppskattning av antalet rader i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Representerar en uppskattning av antalet rader i dokumentet.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Visa aktuellt värde för Lines (uppskattning av antalet rader i dokumentet)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Ange ett nytt värde för Lines-egenskapen
            properties.Lines = 150;
            
            // Lägg till lite innehåll för att demonstrera egenskapens syfte
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Spara arbetsboken
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Obs: Lines-egenskapen är en uppskattning och uppdateras inte automatiskt med faktiskt innehåll
            // Den används främst för dokumentmetadata
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


