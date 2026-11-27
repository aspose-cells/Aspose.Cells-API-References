---
title: "Range.SetOutlineBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Ställer in konturkant runt ett cellområde"
type: docs
url: /sv/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Ställer in konturkant runt ett cellområde.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderEdge | BorderType | Kantkant. |
| borderStyle | CellBorderType | Kantstil. |
| borderColor | CellsColor | Kantfärg. |

### Exempel

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

            // Skapa ett CellsColor‑objekt
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Skapa ett område och sätt högerkant
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Skapa ett annat område och sätt alla kanter
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Spara arbetsboken
            workbook.Save("SetOutlineBorderExample.xlsx");
        }
    }
}
```

### Se även

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Ställer in konturkant runt ett cellområde.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderEdge | BorderType | Kantkant. |
| borderStyle | CellBorderType | Kantstil. |
| borderColor | Färg | Kantfärg. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett cellområde
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Ställ in konturkanter med olika kanttyper och färger
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Spara arbetsboken
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


