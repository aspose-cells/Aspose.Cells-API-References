---
title: "RevisionQueryTable.FieldId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionQueryTable-egenskap. Hämtar ID för det specifika frågetabellfältet som togs bort"
type: docs
url: /sv/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Hämtar ID för det specifika frågetabellfältet som togs bort.

```csharp
public int FieldId { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
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
                // Skapa en frågetabell (detta är ett förenklat exempel)
                // Obs: I ett verkligt scenario måste du skapa en frågetabell först
                // För demonstrationsändamål kommer vi att simulera åtkomst till en RevisionQueryTable

                // Eftersom vi inte kan skapa en RevisionQueryTable direkt i detta förenklade exempel,
                // kommer vi att demonstrera hur man får åtkomst till FieldId‑egenskapen om vi hade en
                // Detta visar mönstret för att läsa den skrivskyddade egenskapen

                // Simulera hämtning av en RevisionQueryTable från revisioner (konceptuellt)
                // I verkligheten skulle du hämta detta från workbook.Revisions eller liknande
                RevisionQueryTable revisionQueryTable = null;

                // Kontrollera om vi har en revisionsfrågetabell (detta är bara för demonstration)
                if (revisionQueryTable != null)
                {
                    // Visa värdet för FieldId‑egenskapen
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Visa andra egenskaper för sammanhang
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Spara arbetsboken
                workbook.Save("FieldIdDemo.xlsx");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


