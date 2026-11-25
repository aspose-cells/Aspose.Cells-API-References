---
title: "Slicer.CaptionVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta se l'intestazione che visualizza il Caption dello slicer è visibile. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.slicers/slicer/captionvisible/
---
## Slicer.CaptionVisible property

Restituisce o imposta se l'intestazione che visualizza il Caption dello slicer è visibile. Il valore predefinito è true

```csharp
[Obsolete("Use Slicer.ShowCaption property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool CaptionVisible { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`ShowCaption`](../showcaption/). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyCaptionVisibleDemo
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
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea una tabella pivot
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi uno slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Imposta le proprietà dello slicer includendo CaptionVisible
            slicer.Caption = "Fruit Selection";
            slicer.CaptionVisible = true; // Show the caption header
            slicer.NumberOfColumns = 2;
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Salva la cartella di lavoro
            workbook.Save("SlicerCaptionVisibleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


