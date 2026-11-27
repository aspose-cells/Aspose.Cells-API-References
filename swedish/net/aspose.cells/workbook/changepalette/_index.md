---
title: "Workbook.ChangePalette"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Ändrar paletten för kalkylbladet på angivet index"
type: docs
url: /sv/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

Ändrar paletten för kalkylbladet på angivet index.

```csharp
public void ChangePalette(Color color, int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | Färgsstruktur. |
| index | Int32 | Palettindex, 0 - 55. |

### Anmärkningar

Paletten har 56 poster, var och en representerad av ett RGB‑värde.

Om du anger en färg som inte finns i paletten, kommer den inte att ha någon effekt.

Så om du vill ange en anpassad färg, ändra paletten först.

Följande är den standardfärgpaletten.

| **Färg** | **Röd** | **Grön** | **Blå** |
| --- | --- | --- | --- |
| Svart | 0 | 0 | 0 |
| Vit | 255 | 255 | 255 |
| Röd | 255 | 0 | 0 |
| Lime | 0 | 255 | 0 |
| Blå | 0 | 0 | 255 |
| Gul | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cyan | 0 | 255 | 255 |
| Mörkröd | 128 | 0 | 0 |
| Grön | 0 | 128 | 0 |
| Marinblå | 0 | 0 | 128 |
| Oliv | 128 | 128 | 0 |
| Lila | 128 | 0 | 128 |
| Turkos | 0 | 128 | 128 |
| Silver | 192 | 192 | 192 |
| Grå | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Color22 | 255 | 128 | 128 |
| Color23 | 0 | 102 | 204 |
| Color24 | 204 | 204 | 255 |
| Color25 | 0 | 0 | 128 |
| Color26 | 255 | 0 | 255 |
| Color27 | 255 | 255 | 0 |
| Color28 | 0 | 255 | 255 |
| Color29 | 128 | 0 | 128 |
| Color30 | 128 | 0 | 0 |
| Color31 | 0 | 128 | 128 |
| Color32 | 0 | 0 | 255 |
| Color33 | 0 | 204 | 255 |
| Color34 | 204 | 255 | 255 |
| Color35 | 204 | 255 | 204 |
| Color36 | 255 | 255 | 153 |
| Color37 | 153 | 204 | 255 |
| Color38 | 255 | 153 | 204 |
| Color39 | 204 | 153 | 255 |
| Color40 | 255 | 204 | 153 |
| Color41 | 51 | 102 | 255 |
| Color42 | 51 | 204 | 204 |
| Color43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodChangePaletteWithColorInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbokinstans
            Workbook workbook = new Workbook();
            
            // Ändra palettfärg vid index 55
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en stil med den modifierade palettfärgen
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


