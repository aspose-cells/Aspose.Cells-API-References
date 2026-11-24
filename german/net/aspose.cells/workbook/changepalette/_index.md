---
title: "Workbook.ChangePalette"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Ändert die Palette für das Tabellenblatt am angegebenen Index"
type: docs
url: /de/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

Ändert die Palette der Tabelle am angegebenen Index.

```csharp
public void ChangePalette(Color color, int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Color-Struktur. |
| Index | Int32 | Palettenindex, 0 - 55. |

### Hinweise

Die Palette hat 56 Einträge, jeder dargestellt durch einen RGB-Wert.

Wenn Sie eine Farbe setzen, die nicht in der Palette ist, wird sie nicht wirksam.

Wenn Sie also eine benutzerdefinierte Farbe festlegen möchten, ändern Sie zuerst die Palette.

Die folgende ist die Standardfarbpalette.

| **Color** | **Red** | **Green** | **Blue** |
| --- | --- | --- | --- |
| Schwarz | 0 | 0 | 0 |
| Weiß | 255 | 255 | 255 |
| Rot | 255 | 0 | 0 |
| Limette | 0 | 255 | 0 |
| Blau | 0 | 0 | 255 |
| Gelb | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cyan | 0 | 255 | 255 |
| Kastanienbraun | 128 | 0 | 0 |
| Grün | 0 | 128 | 0 |
| Marineblau | 0 | 0 | 128 |
| Oliv | 128 | 128 | 0 |
| Lila | 128 | 0 | 128 |
| Türkis | 0 | 128 | 128 |
| Silber | 192 | 192 | 192 |
| Grau | 128 | 128 | 128 |
| Farbe17 | 153 | 153 | 255 |
| Farbe18 | 153 | 51 | 102 |
| Farbe19 | 255 | 255 | 204 |
| Farbe20 | 204 | 255 | 255 |
| Farbe21 | 102 | 0 | 102 |
| Farbe22 | 255 | 128 | 128 |
| Farbe23 | 0 | 102 | 204 |
| Farbe24 | 204 | 204 | 255 |
| Farbe25 | 0 | 0 | 128 |
| Farbe26 | 255 | 0 | 255 |
| Farbe27 | 255 | 255 | 0 |
| Farbe28 | 0 | 255 | 255 |
| Farbe29 | 128 | 0 | 128 |
| Farbe30 | 128 | 0 | 0 |
| Farbe31 | 0 | 128 | 128 |
| Farbe32 | 0 | 0 | 255 |
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

### Beispiele

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
            // Erstelle eine Arbeitsmappeninstanz
            Workbook workbook = new Workbook();
            
            // Palettefarbe bei Index 55 ändern
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Stil mit der geänderten Palettefarbe
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


