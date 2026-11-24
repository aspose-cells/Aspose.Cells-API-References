---
title: "Range.SetOutlineBorders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Setzt die Umrandungsrahmen um einen Range von Zellen mit demselben Rahmenstil und derselben Farbe"
type: docs
url: /de/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Setzt die Umrissrahmen um einen Zellenbereich mit demselben Rahmenstil und derselben Farbe.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | CellBorderType | Randstil. |
| borderColor | CellsColor | Randfarbe. |

### Beispiele

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

            // Erstelle ein CellsColor-Objekt mit einer Themenfarbe
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Erstelle einen Range und setze die Umrandungsrahmen
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Speichere die Arbeitsmappe
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Setzt die Umrissrahmen um einen Zellenbereich mit demselben Rahmenstil und derselben Farbe.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | CellBorderType | Randstil. |
| borderColor | Farbe | Randfarbe. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Range von Zellen (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Fülle den Range mit einigen Daten, um die Rahmen sichtbar zu machen
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Rufe SetOutlineBorders mit mittlerem Rahmenstil und roter Farbe auf
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
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

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Setzt äußere Rahmen um einen Zellenbereich.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Rahmenstile. |
| borderColors | Color[] | Rahmenfarben. |

### Hinweise

Sowohl die Länge von borderStyles als auch von borderStyles muss 4 betragen. Die Reihenfolge von borderStyles und borderStyles muss top,bottom,left,right sein.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Zellbereich (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Bereite Rahmenstile und Farben vor
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
                // Setze Konturrahmen mit unterschiedlichen Stilen und Farben
                range.SetOutlineBorders(borderStyles, borderColors);

                // Fülle Zellen mit Daten, um die Rahmen sichtbar zu machen
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


