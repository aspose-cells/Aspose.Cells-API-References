---
title: "Klass RevisionAutoFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionAutoFormat klass. representerar en revisionspost med information om en formateringsändring"
type: docs
url: /sv/net/aspose.cells.revisions/revisionautoformat/
---
## RevisionAutoFormat class

Representerar en revisionspost med information om en formateringsändring.

```csharp
public class RevisionAutoFormat : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionautoformat/cellarea/) { get; } | Hämtar platsen där formateringen tillämpades. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionautoformat/type/) { get; } | Hämtar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionAutoFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
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
                Console.WriteLine($"Error working with RevisionAutoFormat: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


