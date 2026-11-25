---
title: "CellArea.EndRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Campo CellArea. Ottiene o imposta la riga finale di quest'area"
type: docs
url: /it/net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Ottiene o imposta la riga finale di quest'area.

```csharp
public int EndRow;
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Dimostra l'uso di EndRow
            Console.WriteLine("Pivot table ends at row: " + pivotTable.TableRange2.EndRow);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTable_EndRow_Demo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


