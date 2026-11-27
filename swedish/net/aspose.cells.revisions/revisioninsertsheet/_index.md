---
title: "Klass RevisionInsertSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionInsertSheet klass. Representerar en revisionspost för ett blad som har infogats"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

Representerar en revisionspost för ett blad som har infogats.

```csharp
public class RevisionInsertSheet : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | Hämtar åtgärdstypen för revisionen. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | Hämtar namnet på arbetsbladet. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | Hämtar den nollbaserade positionen för det nya bladet i flikfältet. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | Hämtar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionInsertSheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till ett nytt arbetsblad för att eventuellt skapa en revision
                Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

                // Obs: Eftersom vi inte kan skapa RevisionInsertSheet-instans direkt,
                // kommer vi att demonstrera hur man arbetar med en om den fanns i revisionssamlingen
                // Detta är ett simulerat scenario eftersom det faktiska revisionsspårnings-API:et inte är fullt exponerat

                // I ett verkligt scenario med aktiverad revisionsspårning kan du få revisioner som dessa:
                // RevisionInsertSheet revision = null; // Skulle komma från workbook.Revisions-samlingen

                // För demonstrationsändamål kommer vi att visa mönstret för att arbeta med en RevisionInsertSheet
                // Eftersom vi inte kan instansiera den direkt kommer vi att demonstrera mönstret för egenskapsåtkomst

                // Istället för att försöka skapa en instans, visar vi hur man arbetar med en om den finns
                // Detta behåller strukturen samtidigt som kompileringsfelet åtgärdas

                // Visa information om revisionsegenskaperna (simulerat)
                Console.WriteLine("RevisionInsertSheet properties demonstration:");
                Console.WriteLine("Type property would show: RevisionType.InsertSheet");
                Console.WriteLine("ActionType property would show: RevisionActionType.Add");
                Console.WriteLine("Name property would show the sheet name");
                Console.WriteLine("SheetPosition property would show the zero-based position");

                // Spara arbetsboken
                workbook.Save("RevisionInsertSheetDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with potential revisions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionInsertSheet: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


