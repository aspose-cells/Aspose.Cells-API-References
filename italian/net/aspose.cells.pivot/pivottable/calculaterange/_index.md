---
title: "PivotTable.CalculateRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Calcola l'intervallo delle tabelle pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Calcola l'intervallo della PivotTable.

```csharp
public void CalculateRange()
```

### Osservazioni

Se questo metodo non è stato chiamato, forse l'intervallo della tabella pivot non è corretto.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio al primo foglio di lavoro
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B3"].PutValue(2000);
            dataSheet.Cells["A4"].PutValue("Orange");
            dataSheet.Cells["B4"].PutValue(3000);

            // Aggiungi una tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Aggiungi campi di riga e di dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Calcola l'intervallo e aggiorna i dati
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableCalculateRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


