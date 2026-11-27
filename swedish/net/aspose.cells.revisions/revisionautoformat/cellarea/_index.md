---
title: "RevisionAutoFormat.CellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionAutoFormat‑egenskap. Hämtar platsen där formateringen tillämpades"
type: docs
url: /sv/net/aspose.cells.revisions/revisionautoformat/cellarea/
---
## RevisionAutoFormat.CellArea property

Hämtar platsen där formateringen tillämpades.

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

    public class RevisionAutoFormatPropertyCellAreaDemo
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
                    // Demonstrera CellArea-egenskapen (skrivskyddad)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


