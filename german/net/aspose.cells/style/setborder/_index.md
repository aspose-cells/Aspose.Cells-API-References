---
title: "Style.SetBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Setzt die Ränder des Stils"
type: docs
url: /de/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Setzt die Ränder des Stils.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderType | BorderType | Der/die zu setzenden Rand/Ränder können eine Kombination aus [`BorderType`](../../bordertype/) sein. |
| borderStyle | CellBorderType | Der Stil des Randes. |
| borderColor | Farbe | Die Farbe des Randes. |

### Rückgabewert

Ob die aktuellen Rand-Einstellungen geändert wurden.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            var range = worksheet.Cells.CreateRange("A1:D4");

            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            workbook.Save("BorderExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Setzt die Ränder des Stils.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderType | BorderType | Der/die zu setzenden Rand/Ränder können eine Kombination aus [`BorderType`](../../bordertype/) sein. |
| borderStyle | CellBorderType | Der Stil des Randes. |
| borderColor | CellsColor | Die Farbe des Randes. |

### Rückgabewert

Ob die aktuellen Rand-Einstellungen geändert wurden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Erstellen Sie einen Stil
                Style style = workbook.CreateStyle();
                
                // Erstellen Sie ein CellsColor-Objekt mit der entsprechenden Fabrikmethode
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // Rufen Sie SetBorder mit den Parametern BorderType, CellBorderType und CellsColor auf
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Wende den Stil auf eine Zelle an
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Speichere die Arbeitsmappe
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


