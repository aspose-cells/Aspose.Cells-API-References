---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableFormatCollection metod. Formaterar markerat område"
type: docs
url: /sv/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Formaterar markerat område.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | PivotFieldType | The region of the PivotTable to which this rule applies. |
| fieldPosition | Int32 | Position of the field within the axis to which this rule applies. |
| subtotalType | PivotFieldSubtotalType | Subtotalfiltertypen för pivottfältet |
| selectionType | PivotTableSelectionType | Anger hur data ska väljas. |
| isGrandRow | Boolean | Anger om grand total-rader väljs. |
| isGrandColumn | Boolean | Anger om grand total-kolumner väljs. |
| style | Stil | Stilen som tillämpas på pivottabellens område. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från källfil
            Workbook workbook = new Workbook("example.xlsx");
            
            // Kom åt pivottabellen
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Skapa en stil för formatering
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Formatera pivottabellens område
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


