---
title: "Range.CurrentRegion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Returnerar ett Range-objekt som representerar den aktuella regionen. Den aktuella regionen är ett område som begränsas av någon kombination av tomma rader och tomma kolumner"
type: docs
url: /sv/net/aspose.cells/range/currentregion/
---
## Range.CurrentRegion property

Returnerar ett Range-objekt som representerar den aktuella regionen. Den aktuella regionen är ett område som begränsas av en kombination av tomma rader och tomma kolumner.

```csharp
public Range CurrentRegion { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyCurrentRegionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data med några tomma celler för att skapa regioner
            worksheet.Cells["A1"].PutValue("Region 1");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Lämna rad 5 tom för att separera regioner
            
            worksheet.Cells["A6"].PutValue("Region 2");
            worksheet.Cells["A7"].PutValue("Data 4");
            worksheet.Cells["B7"].PutValue("Data 5");
            worksheet.Cells["A8"].PutValue("Data 6");

            // Hämta en cell i den första regionen och konvertera till Range
            Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
            Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
            
            Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
            Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);

            // Hämta en cell i den andra regionen och konvertera till Range
            Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
            Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
            
            Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
            Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);

            // Applicera formatering på hela den aktuella regionen
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            currentRegion1.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


