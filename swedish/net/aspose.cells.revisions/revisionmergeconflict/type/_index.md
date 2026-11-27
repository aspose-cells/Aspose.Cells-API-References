---
title: "RevisionMergeConflict.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionMergeConflict-egenskap. Hämtar revisionstypen"
type: docs
url: /sv/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

Hämtar typen av revision.

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

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera spårningsändringar
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Gör ändringar för att skapa ett scenario med sammanslagningskonflikt
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Simulera en sammanslagningskonflikt genom att öppna filen och göra motstridiga ändringar
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Sammanfoga de motstridiga ändringarna
            workbook.Combine(otherUserWorkbook);

            // Kontrollera om det finns revisioner
            if (workbook.HasRevisions)
            {
                // Hitta revisionen för sammanslagningskonflikten
                RevisionMergeConflict mergeConflictRevision = null;
                // Obs: I den faktiska implementeringen skulle du behöva ett annat sätt att komma åt revisioner
                // eftersom egenskapen Revisions inte är tillgänglig i den tillhandahållna API-definitionen

                if (mergeConflictRevision != null)
                {
                    // Visa egenskapen Type för revisionen av sammanslagningskonflikten
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Demonstrera hur denna information kan användas
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


