---
title: "Enum CellBorderType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellBorderType enum. Enumererar en cells kanttyp"
type: docs
url: /sv/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Enumererar en cells kanttyp.

```csharp
public enum CellBorderType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DashDot | `9` | Representerar tunn streck-punktad linje. |
| DashDotDot | `11` | Representerar tunn streck-punkt-punktad linje. |
| Dashed | `3` | Representerar streckad linje. |
| Dotted | `4` | Representerar streckad linje. |
| Double | `6` | Representerar dubbel linje. |
| Hair | `7` | Representerar hårlinje. |
| MediumDashDot | `10` | Representerar medium streck-punktad linje. |
| MediumDashDotDot | `12` | Representerar medium streck-punkt-punktad linje. |
| MediumDashed | `8` | Representerar medium streckad linje. |
| None | `0` | Representerar ingen linje. |
| Medium | `2` | Representerar medium linje. |
| SlantedDashDot | `13` | Representerar sned medium streck-punktad linje. |
| Thick | `5` | Representerar tjock linje. |
| Thin | `1` | Representerar tunn linje. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett område (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Hämta stil för området
            Style style = workbook.CreateStyle();

            // Ange olika kantstilar för området
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Applicera stilen på området
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Spara arbetsboken
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


