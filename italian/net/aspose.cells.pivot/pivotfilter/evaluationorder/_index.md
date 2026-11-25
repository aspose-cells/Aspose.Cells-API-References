---
title: "PivotFilter.EvaluationOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilter. Ottiene l'Ordine di valutazione del filtro pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/evaluationorder/
---
## PivotFilter.EvaluationOrder property

Ottiene l'ordine di valutazione del filtro pivot.

```csharp
public int EvaluationOrder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyEvaluationOrderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola dati di esempio
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // Crea tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivots[pivotIndex];
            
            // Aggiungi campi
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi filtro pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            
            // Imposta le proprietà del filtro includendo EvaluationOrder
            filter.EvaluationOrder = 1;
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Aggiorna la tabella pivot
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva cartella di lavoro
            book.Save("PivotFilterEvaluationOrderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


