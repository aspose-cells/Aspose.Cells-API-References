---
title: "PivotField.Function"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField proprietà. Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyFunctionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 120;
            cells["A4"].Value = "A";
            cells["B4"].Value = 80;
            cells["A5"].Value = "B";
            cells["B5"].Value = 60;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Aggiungi il campo dati e imposta la funzione su Max
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[fieldIndex];
            dataField.Function = ConsolidationFunction.Max;

            // Calcola tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldFunctionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


