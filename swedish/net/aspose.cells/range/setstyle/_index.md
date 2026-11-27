---
title: "Range.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Applicera cellstilen"
type: docs
url: /sv/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Applicera cellstilen.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Cellstilen. |
| explicitFlag | Boolean | True, endast skriva över formatering som är explicit inställd. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Ställer in stilen för området.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Style-objektet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // Tillämpa stilen på en cell
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // Skapa ett område och applicera samma stil
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


