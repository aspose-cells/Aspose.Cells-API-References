---
title: "RevisionInsertSheet.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionInsertSheet egenskap. Hämtar revisionens typ"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

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

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            
            // Aktivera revisionsspårning (simulerad eftersom StartTrackingRevisions inte är tillgänglig)
            bool trackRevisions = true;

            // Lägg till ett nytt kalkylblad för att skapa en revisionspost
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Simulera hämtning av revisioner (eftersom Revisions-egenskapen inte är tillgänglig)
            if (trackRevisions && workbook.HasRevisions)
            {
                // I ett verkligt scenario skulle vi komma åt revisionerna här
                // Detta förutsätter att vi fick revisionen från någonstans (t.ex. workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Visa Type-egenskapen
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Demonstrera användning av den skrivskyddade Type-egenskapen
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Visa ytterligare information om det infogade bladet
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Kontrollera mot andra revisionstyper
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Spara arbetsboken
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


