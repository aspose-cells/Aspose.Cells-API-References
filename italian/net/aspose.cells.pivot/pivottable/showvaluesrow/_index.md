---
title: "PivotTable.ShowValuesRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se mostra la riga dei valori"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Indica se mostrare la riga dei valori.

```csharp
public bool ShowValuesRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowValuesRowDemo
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
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity as data
            
            // Dimostra la proprietà ShowValuesRow
            Console.WriteLine("Initial ShowValuesRow: " + pivotTable.ShowValuesRow);
            pivotTable.ShowValuesRow = true;
            Console.WriteLine("After setting to true: " + pivotTable.ShowValuesRow);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowValuesRowDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


