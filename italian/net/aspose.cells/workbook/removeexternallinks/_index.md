---
title: "Workbook.RemoveExternalLinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Rimuove tutti i collegamenti esterni nel workbook"
type: docs
url: /it/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Rimuove tutti i collegamenti esterni nel workbook.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo ExternalLinkCollection.Clear(). Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Chiama il metodo RemoveExternalLinks
                workbook.RemoveExternalLinks();

                // Visualizza i risultati o gli effetti della chiamata al metodo
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Salva il workbook se sono state apportate modifiche
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


