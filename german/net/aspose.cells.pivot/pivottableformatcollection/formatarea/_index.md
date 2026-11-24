---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableFormatCollection‑Methode. Formatiert den ausgewählten Bereich"
type: docs
url: /de/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Formatiert den ausgewählten Bereich.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | PivotFieldType | Der Bereich der PivotTable, für den diese Regel gilt. |
| fieldPosition | Int32 | Position des Feldes innerhalb der Achse, für die diese Regel gilt. |
| subtotalType | PivotFieldSubtotalType | Der Zwischensummen-Filtertyp des Pivot-Feldes |
| selectionType | PivotTableSelectionType | Gibt an, wie Daten ausgewählt werden. |
| isGrandRow | Boolean | Gibt an, ob Gesamtsummen‑Zeilen ausgewählt werden. |
| isGrandColumn | Boolean | Gibt an, ob Gesamtsummen‑Spalten ausgewählt werden. |
| Stil | Stil | Der Stil, der auf den Bereich der Pivot-Tabelle angewendet wird. |

### Beispiele

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
            // Ein Arbeitsbuch aus einer Quelldatei erstellen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Zugriff auf die PivotTable
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Erstelle einen Stil für die Formatierung
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Formatieren Sie den Pivot-Tabellenbereich
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


