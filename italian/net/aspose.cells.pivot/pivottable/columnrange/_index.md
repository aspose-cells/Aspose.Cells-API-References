---
title: "PivotTable.ColumnRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area colonna nel report PivotTable. Sola lettura"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/columnrange/
---
## PivotTable.ColumnRange property

Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area colonna nel report PivotTable. Sola lettura.

```csharp
public CellArea ColumnRange { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnRangeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;
            
            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aggiorna i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ottieni l'intervallo di colonna della tabella pivot
            CellArea columnRange = pivotTable.ColumnRange;
            Console.WriteLine("Pivot Table Column Range: " + columnRange);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableColumnRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


