---
title: "Classe DeleteOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DeleteOptions. Rappresenta l'impostazione per l'eliminazione di righe/colonne"
type: docs
url: /it/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Rappresenta l'impostazione per l'eliminazione di righe/colonne.

```csharp
public class DeleteOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Ottiene/imposta il monitor per il tracciamento delle modifiche causate dall'eliminazione. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Visualizza i dati originali
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Crea DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Elimina la seconda riga (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Visualizza i dati dopo l'eliminazione
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Salva la cartella di lavoro
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


