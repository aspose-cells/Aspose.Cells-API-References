---
title: "Classe RevisionAutoFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionAutoFormat class. rappresenta un record di revisione delle informazioni su una modifica di formattazione"
type: docs
url: /it/net/aspose.cells.revisions/revisionautoformat/
---
## RevisionAutoFormat class

rappresenta un record di revisione delle informazioni su una modifica di formattazione.

```csharp
public class RevisionAutoFormat : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionautoformat/cellarea/) { get; } | Ottiene la posizione in cui è stata applicata la formattazione. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionautoformat/type/) { get; } | Ottiene il tipo della revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla raccolta dei log delle revisioni
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Trova la prima istanza di RevisionAutoFormat
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
                    // Dimostra la proprietà Type (sola lettura)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");

                    // Dimostra la proprietà CellArea (sola lettura)
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

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


