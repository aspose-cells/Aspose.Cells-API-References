---
title: "Worksheet.Outline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la struttura di contorno in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Ottiene la struttura in questo foglio di lavoro.

```csharp
public Outline Outline { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e crea gruppi di contorno
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Raggruppa righe (crea contorno)
            worksheet.Cells.GroupRows(0, 9, false);

            // Accedi alle proprietà del contorno
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Modifica le impostazioni del contorno
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Separa i raggruppamenti delle righe per dimostrare la funzionalità del contorno
            worksheet.Cells.UngroupRows(0, 9);

            // Salva la cartella di lavoro
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


