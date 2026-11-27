---
title: "Enum RevisionActionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionActionType-enum. Representerar typen av revisionsåtgärd"
type: docs
url: /sv/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Representerar typen av revisionsåtgärd.

```csharp
public enum RevisionActionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Add | `0` | Lägg till revision. |
| Delete | `1` | Ta bort revision. |
| DeleteColumn | `2` | Kolumnborttagningsrevision. |
| DeleteRow | `3` | Radborttagningsrevision. |
| InsertColumn | `4` | Kolumninfogningsrevision. |
| InsertRow | `5` | Radinfogning revision. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Utför olika operationer som genererar olika revisionstyper
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Kontrollera om arbetsboken har revisioner
            if (workbook.HasRevisions)
            {
                // Obs: Det ursprungliga API:et ger inte direkt åtkomst till revisionssamlingen
                // Så vi kommer bara att demonstrera enumen RevisionActionType som begärt
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // Demonstrera användning av värden i enumen RevisionActionType
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Spara arbetsboken
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


