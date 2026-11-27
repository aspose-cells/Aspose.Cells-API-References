---
title: "RevisionQueryTable.CellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionQueryTable‑egenskap. Hämtar platsen för den påverkade frågetabellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Hämtar platsen för den påverkade frågetabellen.

```csharp
public CellArea CellArea { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // I ett verkligt scenario skulle du hämta revisioner från arbetsboken
                // För demonstration kommer vi att skapa ett konceptuellt exempel
                // Obs: RevisionQueryTable-instansieringar erhålls vanligtvis från arbetsboksrevisioner
                RevisionQueryTable revisionQueryTable = null;

                // Kontrollera om vi har en revisionsfrågetabell
                if (revisionQueryTable != null)
                {
                    // Visa CellArea‑egenskapens värde (skrivskyddad)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Visa andra egenskaper för sammanhang
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Spara arbetsboken
                workbook.Save("CellAreaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


