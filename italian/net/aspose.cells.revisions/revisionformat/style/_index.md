---
title: "RevisionFormat.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionFormat. Restituisce lo stile applicato"
type: docs
url: /it/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Ottiene lo stile applicato.

```csharp
public Style Style { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro (il tracciamento delle revisioni è abilitato per impostazione predefinita quando vengono apportate modifiche)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati e formattazione per creare una revisione
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Creare uno stile e applicarlo alla cella
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Accedi alle revisioni tramite RevisionLogs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Visualizza le proprietà di stile attuali dalla revisione
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Nota: la proprietà Style è di sola lettura in RevisionFormat, quindi non possiamo modificarla direttamente
                        // Per modificare la formattazione, dovremmo modificare direttamente lo stile della cella
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


