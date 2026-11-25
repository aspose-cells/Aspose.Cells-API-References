---
title: "Enum SlicerStyleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Slicers.SlicerStyleType enum. Specifica lo stile della visualizzazione dello slicer"
type: docs
url: /it/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Specifica lo stile della vista slicer

```csharp
public enum SlicerStyleType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | stile chiaro predefinito uno |
| SlicerStyleLight2 | `1` | stile chiaro predefinito due |
| SlicerStyleLight3 | `2` | stile chiaro predefinito tre |
| SlicerStyleLight4 | `3` | stile chiaro predefinito quattro |
| SlicerStyleLight5 | `4` | stile chiaro predefinito cinque |
| SlicerStyleLight6 | `5` | stile chiaro predefinito sei |
| SlicerStyleOther1 | `6` | stile predefinito altro uno |
| SlicerStyleOther2 | `7` | stile predefinito altro due |
| SlicerStyleDark1 | `8` | stile scuro predefinito uno |
| SlicerStyleDark2 | `9` | stile scuro predefinito due |
| SlicerStyleDark3 | `10` | stile scuro predefinito tre |
| SlicerStyleDark4 | `11` | stile scuro predefinito quattro |
| SlicerStyleDark5 | `12` | stile scuro predefinito cinque |
| SlicerStyleDark6 | `13` | stile scuro predefinito sei |
| Custom | `14` | stile definito dall'utente, non supportato per ora |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi slicer
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Imposta lo stile del filtro
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Salva la cartella di lavoro
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


