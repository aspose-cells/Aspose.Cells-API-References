---
title: "PivotTable.PivotFormats"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene tutti i formati di cella applicati a questa tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/pivotformats/
---
## PivotTable.PivotFormats property

Ottiene tutti i formati di cella applicati a questa tabella pivot.

```csharp
public PivotTableFormatCollection PivotFormats { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotFormatsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crea stile per la formattazione
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);

            // Applica la formattazione all'area dati della tabella pivot
            pivotTable.PivotFormats.FormatArea(
                PivotFieldType.Data, 
                0, 
                PivotFieldSubtotalType.None, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithFormats.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


