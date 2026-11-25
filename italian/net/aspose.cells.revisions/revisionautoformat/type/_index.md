---
title: "RevisionAutoFormat.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionAutoFormat. Ottiene il tipo della revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionautoformat/type/
---
## RevisionAutoFormat.Type property

Ottiene il tipo della revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

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
            // Crea un nuovo workbook con tracciamento delle revisioni
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
                    
                    // Mostra il valore enum per chiarezza
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

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


