---
title: "Slicer.LockedPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente"
type: docs
url: /it/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente.

```csharp
public bool LockedPosition { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crea collezione di tabelle pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Crea una tabella pivot
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crea collezione di slicer
            SlicerCollection slicers = worksheet.Slicers;
            
            // Aggiungi uno slicer per la tabella pivot
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Imposta le proprietà dello slicer
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // Dimostra la proprietà LockedPosition
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Imposta LockedPosition su false per consentire lo spostamento
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Salva la cartella di lavoro
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


