---
title: "Slicer.NumberOfColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta il numero di colonne nello slicer. Il valore predefinito è 1"
type: docs
url: /it/net/aspose.cells.slicers/slicer/numberofcolumns/
---
## Slicer.NumberOfColumns property

Restituisce o imposta il numero di colonne nello slicer. Il valore predefinito è 1.

```csharp
public int NumberOfColumns { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Crea dati di esempio per la tabella pivot
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["A2"].Value = "Fruits";
            cells["B2"].Value = "Apple";
            cells["A3"].Value = "Fruits";
            cells["B3"].Value = "Banana";
            cells["A4"].Value = "Vegetables";
            cells["B4"].Value = "Carrot";

            // Crea una tabella pivot - memorizza l'indice quindi ottieni l'oggetto PivotTable
            int pivotIndex = sheet.PivotTables.Add("D1", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Product");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Aggiungi uno slicer collegato alla tabella pivot
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Configura le proprietà dello slicer
            slicer.Caption = "Product Categories";
            slicer.TopPixel = 50;
            slicer.LeftPixel = 50;
            slicer.HeightPixel = 150;
            slicer.WidthPixel = 200;

            // Dimostra la proprietà NumberOfColumns
            slicer.NumberOfColumns = 2;

            // Salva la cartella di lavoro
            workbook.Save("SlicerDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


