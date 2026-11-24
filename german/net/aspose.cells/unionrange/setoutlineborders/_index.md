---
title: "UnionRange.SetOutlineBorders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Setzt Umrandungen um einen Zellbereich"
type: docs
url: /de/net/aspose.cells/unionrange/setoutlineborders/
---
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}

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
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeAColorArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Additional Data");

            // Erstelle einen Bereich und konvertiere ihn zu UnionRange
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            UnionRange unionRange = worksheet.Cells.CreateRange(range.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range });

            try
            {
                // Definiere Rahmenstile und Farben für alle vier Ränder
                CellBorderType[] borderStyles = new CellBorderType[]
                {
                    CellBorderType.Thin,    // Top border
                    CellBorderType.Medium,  // Right border
                    CellBorderType.Thick,   // Bottom border
                    CellBorderType.Double   // Left border
                };

                Color[] borderColors = new Color[]
                {
                    Color.Red,     // Top border color
                    Color.Blue,    // Right border color
                    Color.Green,   // Bottom border color
                    Color.Orange   // Left border color
                };

                // Rufe SetOutlineBorders mit den Arrays auf
                unionRange.SetOutlineBorders(borderStyles, borderColors);

                Console.WriteLine("SetOutlineBorders method called successfully with CellBorderType[] and Color[] parameters");
                Console.WriteLine($"Applied borders to range: {unionRange.RefersTo}");

                // Speichere die Arbeitsmappe
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}

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
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test";
            worksheet.Cells["A2"].Value = "More Data";
            worksheet.Cells["B2"].Value = "Example";

            try
            {
                // Erstelle einen UnionRange, der A1:B2 abdeckt
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Setze Umrissrahmen mit einem bestimmten Rahmentyp und einer Farbe
                unionRange.SetOutlineBorders(CellBorderType.Medium, Color.Blue);

                Console.WriteLine("SetOutlineBorders method called successfully");
                Console.WriteLine($"Border applied to range: {unionRange.RefersTo}");

                // Speichere die Arbeitsmappe
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


