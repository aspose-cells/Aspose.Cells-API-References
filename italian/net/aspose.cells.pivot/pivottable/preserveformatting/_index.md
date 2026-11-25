---
title: "PivotTable.PreserveFormatting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se la formattazione delle celle PivotTableFormat viene preservata quando la PivotTable viene aggiornata o ricalcolata"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Indica se la formattazione delle celle ([`PivotTableFormat`](../../pivottableformat/)) viene preservata quando la PivotTable viene aggiornata o ricalcolata.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.PreserveCellFormattingOnUpdate. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("source.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Abilita la conservazione della formattazione durante l'aggiornamento
            pivotTable.PreserveFormatting = true;
            
            // Applica una certa formattazione all'area dati della tabella pivot
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Formatta l'area dati della tabella pivot
            pivotTable.FormatAll(style);
            
            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


