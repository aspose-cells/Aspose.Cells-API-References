---
title: "Classe InsertOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.InsertOptions. Rappresenta le opzioni di inserimento"
type: docs
url: /it/net/aspose.cells/insertoptions/
---
## InsertOptions class

Rappresenta le opzioni di inserimento.

```csharp
public class InsertOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [InsertOptions](insertoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Ottiene/imposta il monitor per tracciare le modifiche causate dall'inserimento. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Indica se i riferimenti in altri fogli di lavoro verranno aggiornati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Definisci l'area di celle dove verranno inserite le righe
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Inserisci righe con le opzioni specificate
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Salva la cartella di lavoro
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


