---
title: "Workbook.CloseAccessCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Chiude la sessione che utilizza cache per accedere ai dati"
type: docs
url: /it/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Chiude la sessione che utilizza cache per accedere ai dati.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | AccessCacheOptions | opzioni di accesso ai dati |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio e formattazione condizionale
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Aggiungi formattazione condizionale
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Avvia la cache di accesso per la formattazione condizionale
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Accedi alle celle con formattazione condizionale nella cache
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Chiudi la cache di accesso
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


