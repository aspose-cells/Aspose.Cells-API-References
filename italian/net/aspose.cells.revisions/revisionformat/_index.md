---
title: "Classe RevisionFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionFormat classe. Rappresenta un record di revisione delle informazioni su una modifica di formattazione."
type: docs
url: /it/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Rappresenta un record di revisione delle informazioni su una modifica di formattazione.

```csharp
public class RevisionFormat : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | L'intervallo a cui è stata applicata questa formattazione. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Ottiene lo stile applicato. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Ottiene il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro in modalità condivisa per abilitare il tracciamento delle revisioni
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi alcuni dati e applica la formattazione per creare una revisione
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Applica uno stile per creare una revisione di formattazione
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Accedi ai registri delle revisioni
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Visualizza le proprietà della revisione
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Visualizza informazioni sullo stile
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


