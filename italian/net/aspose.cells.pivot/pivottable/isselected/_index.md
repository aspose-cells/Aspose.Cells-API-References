---
title: "PivotTable.IsSelected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se questa PivotTable è selezionata"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Indica se questa PivotTable è selezionata.

```csharp
public bool IsSelected { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
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

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

            // Inizialmente, IsSelected è false
            Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);

            // Seleziona la tabella pivot
            pivotTable.IsSelected = true;
            Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);

            // Deseleziona la tabella pivot
            pivotTable.IsSelected = false;
            Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


