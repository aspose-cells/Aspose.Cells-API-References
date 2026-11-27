---
title: "PivotTable.AltTextDescription"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar beskrivningen av alt-texten"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/alttextdescription/
---
## PivotTable.AltTextDescription property

Hämtar beskrivningen av alternativ text.

```csharp
public string AltTextDescription { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextDescriptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa den aktuella alt-textbeskrivningen
            Console.WriteLine("Current AltTextDescription: " + pivotTable.AltTextDescription);

            // Ange en ny alt-textbeskrivning
            pivotTable.AltTextDescription = "Sales data by product category";

            // Spara arbetsboken
            workbook.Save("PivotTableAltTextDescriptionDemo.xlsx");

            // Visa den nya alt-textbeskrivningen
            Console.WriteLine("New AltTextDescription: " + pivotTable.AltTextDescription);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


