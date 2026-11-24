---
title: "Enum OdsPageBackgroundType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsPageBackgroundType Enum. Repräsentiert den Seitenhintergrundtyp von ODS"
type: docs
url: /de/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

Stellt den Seitenhintergrundtyp von ODS dar.

```csharp
public enum OdsPageBackgroundType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Hintergrund. |
| Color | `1` | Formatiert den Hintergrund mit Farbe. |
| Graphic | `2` | Formatiert den Hintergrund mit Bild. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Seiteneinrichtung des Arbeitsblatts
            PageSetup pageSetup = worksheet.PageSetup;

            // Greift auf die ODSPageBackground-Eigenschaft zu
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Setze den Hintergrundtyp auf Farbe
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Legen Sie die Hintergrundfarbe fest
            odsPageBackground.Color = Color.LightBlue;

            // Speichere die Arbeitsmappe
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


