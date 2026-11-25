---
title: "PivotField.SetSubtotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Imposta come calcolare i subtotali per il campo specificato"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Imposta come subtotale il campo specificato.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | [`PivotFieldSubtotalType`](../../pivotfieldsubtotaltype/) |
| visualizzato | Booleano | Indica se il campo specificato mostra i subtotali. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = sheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = "TV";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Electronics";
            cells["B3"].Value = "Radio";
            cells["C3"].Value = 500;
            
            cells["A4"].Value = "Clothing";
            cells["B4"].Value = "Shirt";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "Clothing";
            cells["B5"].Value = "Pants";
            cells["C5"].Value = 400;

            // Aggiungi tabella pivot
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Aggiungi campi di riga
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Dimostra SetSubtotals con PivotFieldSubtotalType e booleano
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


