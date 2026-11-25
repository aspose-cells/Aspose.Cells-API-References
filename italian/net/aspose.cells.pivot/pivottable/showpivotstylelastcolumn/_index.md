---
title: "PivotTable.ShowPivotStyleLastColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTable property. Indica se la formattazione della colonna è applicata"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showpivotstylelastcolumn/
---
## PivotTable.ShowPivotStyleLastColumn property

Indica se la formattazione della colonna è applicata.

```csharp
public bool ShowPivotStyleLastColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleLastColumnDemo
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

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Imposta lo stile della tabella pivot e mostra lo stile dell'ultima colonna
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            pivotTable.ShowPivotStyleLastColumn = true;

            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowLastColumnStyle.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


