---
title: "RevisionQueryTable.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionQueryTable‑egenskap. Representerar revisionens typ"
type: docs
url: /sv/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

Representerar typen av revisionen.

```csharp
public override RevisionType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyTypeDemo
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

                // Skapa en mock RevisionQueryTable (detta är konceptuellt – i verkligheten skulle du hämta från revisioner)
                // Eftersom vi inte kan instansiera RevisionQueryTable direkt, kommer vi att demonstrera mönstret
                RevisionQueryTable revisionQueryTable = null;

                // Kontrollera om vi har en revisionsfrågetabell
                if (revisionQueryTable != null)
                {
                    // Visa Type‑egenskapens värde (skrivskyddad)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Visa enum‑värdet som heltal för referens
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Visa andra egenskaper för sammanhang
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Spara arbetsboken
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


