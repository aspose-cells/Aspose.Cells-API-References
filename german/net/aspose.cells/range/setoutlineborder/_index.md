---
title: "Range.SetOutlineBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Setzt einen Umrandungsrahmen um einen Zellbereich"
type: docs
url: /de/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Setzt den Umrissrahmen um einen Zellenbereich.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderEdge | BorderType | Randkante. |
| borderStyle | CellBorderType | Randstil. |
| borderColor | CellsColor | Randfarbe. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle ein CellsColor-Objekt
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Erstelle einen Bereich und setze den rechten Rand
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Erstelle einen weiteren Bereich und setze alle Ränder
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Speichere die Arbeitsmappe
            workbook.Save("SetOutlineBorderExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Setzt den Umrissrahmen um einen Zellenbereich.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderEdge | BorderType | Randkante. |
| borderStyle | CellBorderType | Randstil. |
| borderColor | Farbe | Randfarbe. |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Zellbereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Setze Umrandungsrahmen mit verschiedenen Randtypen und -farben
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Speichere die Arbeitsmappe
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


