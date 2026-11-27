---
title: "QueryTable.PreserveFormatting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTable-egenskap. Returnerar eller anger PreserveFormatting för objektet"
type: docs
url: /sv/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Returnerar eller anger PreserveFormatting för objektet.

```csharp
public bool PreserveFormatting { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och formatering
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Tillämpa formatering på dataområdet
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Tillämpa stil på varje cell i området
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Skapa en frågetabell (simulerad eftersom faktisk skapning kräver extern datakälla)
            // I verklig användning skulle du skapa detta från en extern anslutning
            QueryTable queryTable = worksheet.QueryTables[0];

            // Visa aktuellt PreserveFormatting‑värde
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // Ställ in PreserveFormatting till false (bevarar inte befintlig formatering vid uppdatering)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simulera uppdatering av frågetabellen (rensar normalt formatering när PreserveFormatting är false)
            // I ett verkligt scenario skulle detta ske när frågetabellen uppdaterar sina data
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // Ställ in PreserveFormatting tillbaka till true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simulera uppdatering igen (bevarar nu formatering)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Spara arbetsboken
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### Se även

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


