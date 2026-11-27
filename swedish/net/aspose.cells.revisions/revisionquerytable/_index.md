---
title: "Klass RevisionQueryTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionQueryTable-klass. Representerar en revision av en förändring av ett frågetabellfält"
type: docs
url: /sv/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Representerar en revision av en ändring i en frågetabells fält.

```csharp
public class RevisionQueryTable : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Hämtar platsen för den påverkade frågetabellen. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Hämtar ID för det specifika frågetabellfältet som togs bort. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Representerar typen av revisionen. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata för att skapa ett sammanhang för frågetabellen
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Obs: RevisionQueryTable-instansieringar erhålls vanligtvis från arbetsboksrevisioner
                // Detta är en konceptuell demonstration eftersom vi inte kan instansiera RevisionQueryTable direkt

                // I ett verkligt scenario skulle du komma åt revisioner så här:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Åtkomst till egenskaper
                //     }
                // }

                // För demonstration kommer vi att visa hur man arbetar med RevisionQueryTable-egenskaper
                // om vi hade en instans
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Spara arbetsboken
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


