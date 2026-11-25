---
title: "PivotTable.ColumnHeaderCaption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene e imposta il Caption personalizzato dell'intestazione di colonna della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/columnheadercaption/
---
## PivotTable.ColumnHeaderCaption property

Ottiene e imposta la didascalia personalizzata dell'intestazione di colonna della PivotTable.

```csharp
public string ColumnHeaderCaption { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnHeaderCaptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["A3"].Value = "Bike";
            cells["A4"].Value = "Car";
            cells["A5"].Value = "Car";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Aggiungi una tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Quarter
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Imposta la didascalia dell'intestazione di colonna
            PivotField columnField = pivotTable.ColumnFields[0];
            pivotTable.ColumnHeaderCaption = "Quarter Header";
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableColumnHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


