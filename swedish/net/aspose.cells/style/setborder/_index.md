---
title: "Style.SetBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Anger kantlinjerna för stilen"
type: docs
url: /sv/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Ställer in kanterna för stilen.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderType | BorderType | De kantlinjer som ska sättas kan vara en kombination av [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | Stilen på kantlinjen. |
| borderColor | Färg | Färgen på kantlinjen. |

### Returvärde

Om de aktuella kantinställningarna har ändrats.

### Exempel

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

### Se även

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Ställer in kanterna för stilen.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderType | BorderType | De kantlinjer som ska sättas kan vara en kombination av [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | Stilen på kantlinjen. |
| borderColor | CellsColor | Färgen på kantlinjen. |

### Returvärde

Om de aktuella kantinställningarna har ändrats.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Skapa en stil
                Style style = workbook.CreateStyle();
                
                // Skapa ett CellsColor-objekt med hjälp av rätt fabriksmetod
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // Anropa SetBorder med parametrarna BorderType, CellBorderType och CellsColor
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Tillämpa stilen på en cell
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Spara arbetsboken
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

### Se även

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


