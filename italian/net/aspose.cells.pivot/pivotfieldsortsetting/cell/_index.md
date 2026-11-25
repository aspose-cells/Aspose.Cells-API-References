---
title: "PivotFieldSortSetting.Cell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldSortSetting. Ordina per i valori nella riga o nella colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsortsetting/cell/
---
## PivotFieldSortSetting.Cell property

Ordina per i valori nella riga o colonna.

```csharp
public string Cell { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyCellDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 5;
            cells["B4"].Value = 8;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ordina per riferimento di cella
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A2");
            
            // Dimostra l'uso della proprietà Cell
            Console.WriteLine("Sorting by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Modifica la cella di ordinamento
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A3");
            Console.WriteLine("Changed sort cell to: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Cancella l'ordinamento delle celle
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            Console.WriteLine("After clearing cell sort: " + 
                (string.IsNullOrEmpty(pivotTable.RowFields[0].SortSetting.Cell) ? "Empty" : "Has value"));
        }
    }
}
```

### Vedi anche

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


