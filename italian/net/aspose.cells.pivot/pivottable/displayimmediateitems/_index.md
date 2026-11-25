---
title: "PivotTable.DisplayImmediateItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se gli elementi nelle aree di riga e colonna sono visibili quando l'area dati della PivotTable è vuota. Il valore predefinito è vero."
type: docs
url: /it/net/aspose.cells.pivot/pivottable/displayimmediateitems/
---
## PivotTable.DisplayImmediateItems property

Indica se gli elementi nelle aree riga e colonna sono visibili quando l'area dati della PivotTable è vuota. Il valore predefinito è true.

```csharp
public bool DisplayImmediateItems { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayImmediateItemsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
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
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Dimostra la proprietà DisplayImmediateItems
            Console.WriteLine("Initial DisplayImmediateItems value: " + pivotTable.DisplayImmediateItems);
            
            // Modifica il valore della proprietà
            pivotTable.DisplayImmediateItems = false;
            Console.WriteLine("After setting to false: " + pivotTable.DisplayImmediateItems);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDisplayImmediateItemsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


