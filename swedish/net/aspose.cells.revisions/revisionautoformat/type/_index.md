---
title: "RevisionAutoFormat.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionAutoFormat‑egenskap. Hämtar typen av revision"
type: docs
url: /sv/net/aspose.cells.revisions/revisionautoformat/type/
---
## RevisionAutoFormat.Type property

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

    public class RevisionAutoFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till revisionsloggssamlingen
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                // Hitta den första RevisionAutoFormat-instansen
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Demonstrera Type-egenskapen (skrivskyddad)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");
                    
                    // Visa enum‑värdet för tydlighet
                    Console.WriteLine($"Revision type value: {(int)type}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
                }
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
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


