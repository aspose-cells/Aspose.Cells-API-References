---
title: "RevisionInsertSheet.ActionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionInsertSheet egenskap. Hämtar åtgärdstypen för revisionen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Hämtar åtgärdstypen för revisionen.

```csharp
public RevisionActionType ActionType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            // Obs: StartTrackingRevisions är inte tillgänglig i det medföljande API:et
            // workbook.StartTrackingRevisions();

            // Lägg till ett nytt kalkylblad för att skapa en revisionspost
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Obs: StopTrackingRevisions är inte tillgänglig i det medföljande API:et
            // workbook.StopTrackingRevisions();
            
            // Obs: Revisions-egenskapen är inte tillgänglig i det medföljande API:et
            // Vi kommer att använda HasRevisions för att kontrollera om det finns några revisioner
            if (workbook.HasRevisions)
            {
                // I ett verkligt scenario skulle vi komma åt revisionerna här
                // Eftersom vi inte kan skapa RevisionInsertSheet direkt, kommer vi att simulera att kontrollera en
                // Detta förutsätter att vi fick revisionen från någonstans (t.ex. workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // Eftersom vi inte kan skapa eller sätta ActionType, kommer vi bara att demonstrera hur man kontrollerar den
                if (insertSheetRevision != null)
                {
                    // Visa ActionType-egenskapen
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Demonstrera användning av den skrivskyddade egenskapen
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Spara arbetsboken med revisioner
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### Se även

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


