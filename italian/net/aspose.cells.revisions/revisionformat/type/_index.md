---
title: "RevisionFormat.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionFormat. Restituisce il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Ottiene il tipo di revisione.

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

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro in modalità condivisa per abilitare il tracciamento delle revisioni
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati e applica la formattazione per creare una revisione
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Applica uno stile per creare una revisione di formattazione
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Accedi ai registri delle revisioni
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Visualizza il valore della proprietà Type
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Mostra informazioni aggiuntive sulla revisione
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


