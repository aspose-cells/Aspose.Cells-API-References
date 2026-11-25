---
title: "Enum UpdateLinksType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.UpdateLinksType enum. Rappresenta come aggiornare i collegamenti ad altri cartelle di lavoro quando la cartella di lavoro è aperta"
type: docs
url: /it/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Rappresenta come aggiornare i collegamenti ad altre cartelle di lavoro quando la cartella di lavoro è aperta.

```csharp
public enum UpdateLinksType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| UserSet | `0` | Richiedi all'utente di aggiornare. |
| Never | `1` | Non aggiornare e non richiedere all'utente. |
| Always | `2` | Aggiorna sempre. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta UpdateLinksType su Aggiorna sempre
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Salva la cartella di lavoro
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Output dell'impostazione corrente di UpdateLinksType
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


