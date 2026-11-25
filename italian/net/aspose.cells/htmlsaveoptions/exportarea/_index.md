---
title: "HtmlSaveOptions.ExportArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta l'area CellArea da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in HTML."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Ottiene o imposta l'area CellArea da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata sarà esportata durante il salvataggio del file in html.

```csharp
public CellArea ExportArea { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati nel foglio di lavoro
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Imposta le opzioni di salvataggio HTML con area di esportazione
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Salva la cartella di lavoro con l'area di esportazione specificata
            workbook.Save("output.html", options);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


