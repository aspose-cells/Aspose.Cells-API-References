---
title: "PivotTable.ClearData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Cancella i dati e la formattazione della vista PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Cancella i dati e la formattazione della visualizzazione della PivotTable.

```csharp
public void ClearData()
```

### Osservazioni

Se questo metodo non viene chiamato prima di aggiungere o eliminare PivotField, potrebbe succedere che i dati della PivotTable non siano corretti

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodClearDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(15);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table with data:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Cancella i dati della tabella pivot
            pivotTable.ClearData();
            Console.WriteLine("\nAfter ClearData():");
            Console.WriteLine("Pivot table row count: " + (pivotTable.DataBodyRange.EndRow - pivotTable.DataBodyRange.StartRow + 1));

            // Ricostruisci la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nRebuilt pivot table:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Salva cartella di lavoro
            workbook.Save("PivotTableClearDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


