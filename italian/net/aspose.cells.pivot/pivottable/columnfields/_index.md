---
title: "PivotTable.ColumnFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce un oggetto PivotFields che sono attualmente mostrati come campi di colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Restituisce un oggetto PivotFields che è attualmente mostrato come campi colonna.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnFieldsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Bikes";
            cells["B3"].Value = 200;
            cells["A4"].Value = "Cars";
            cells["B4"].Value = 300;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 400;
            cells["A6"].Value = "Trucks";
            cells["B6"].Value = 500;

            // Aggiungi tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi di riga e di colonna
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Sales");

            // Accedi e manipola il campo di colonna
            PivotField columnField = pivotTable.ColumnFields[0];
            columnField.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);

            // Calcola e aggiorna i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableColumnFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


