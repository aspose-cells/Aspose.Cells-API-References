---
title: "Slicer.AddPivotConnection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Slicer. Aggiunge la connessione PivotTable"
type: docs
url: /it/net/aspose.cells.slicers/slicer/addpivotconnection/
---
## Slicer.AddPivotConnection method

Aggiunge una connessione PivotTable.

```csharp
public void AddPivotConnection(PivotTable pivot)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | L'oggetto PivotTable |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodAddPivotConnectionWithPivotTableDemo
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
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Aggiungi slicer - parametri corretti
            int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Aggiungi connessione pivot allo slicer
            slicer.AddPivotConnection(pivotTable);

            // Salva la cartella di lavoro
            workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


