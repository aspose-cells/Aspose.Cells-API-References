---
title: "Range.SetOutlineBorders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Anger konturkanterna runt ett cellområde med samma kantstil och färg"
type: docs
url: /sv/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Ställer in konturkanterna runt ett cellområde med samma kantstil och färg.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | CellBorderType | Kantstil. |
| borderColor | CellsColor | Kantfärg. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa ett CellsColor-objekt med en temafärg
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Skapa ett område och ange konturkanter
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Spara arbetsboken
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Ställer in konturkanterna runt ett cellområde med samma kantstil och färg.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | CellBorderType | Kantstil. |
| borderColor | Färg | Kantfärg. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett cellområde (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Fyll området med lite data så att kanterna blir synliga
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Anropa SetOutlineBorders med medium kantstil och röd färg
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Spara arbetsboken för att se effekten
                workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Ställer in konturkanter runt ett cellområde.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Kantstilar. |
| borderColors | Color[] | Kantfärger. |

### Anmärkningar

Både längden på borderStyles och borderStyles måste vara 4. Ordningen på borderStyles och borderStyles måste vara top,bottom,left,right

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett cellområde (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Förbered kantstilar och färger
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dashed,
                CellBorderType.Double,
                CellBorderType.MediumDashDot
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // Ställ in konturkanter med olika stilar och färger
                range.SetOutlineBorders(borderStyles, borderColors);

                // Fyll cellerna med data så att kanterna blir synliga
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Spara arbetsboken
                workbook.Save("RangeSetOutlineBordersDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


