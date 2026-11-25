---
title: "PivotTable.ShowPivotStyleColumnHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se l'intestazione di colonna nella tabella pivot deve avere lo stile applicato"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showpivotstylecolumnheader/
---
## PivotTable.ShowPivotStyleColumnHeader property

Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato.

```csharp
public bool ShowPivotStyleColumnHeader { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnHeaderDemo
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
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Imposta lo stile della tabella pivot
            pivotTable.ShowPivotStyleColumnHeader = true;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowPivotStyleColumnHeaderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


