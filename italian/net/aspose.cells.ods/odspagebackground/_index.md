---
title: "Classe OdsPageBackground"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OdsPageBackground classe. Rappresenta lo sfondo della pagina ODS"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

Rappresenta lo sfondo della pagina di ODS.

```csharp
public class OdsPageBackground
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Ottiene e imposta il colore dello sfondo. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Ottiene e imposta i dati grafici. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Ottiene e imposta la posizione della grafica di sfondo. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Ottiene e imposta il tipo di grafica di sfondo della pagina. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Indica se è una grafica collegata. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Ottiene e imposta il percorso della grafica collegata. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Ottiene e imposta il tipo di sfondo della pagina. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accedi all'oggetto PageSetup
            PageSetup pageSetup = sheet.PageSetup;

            // Accedi all'oggetto ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Imposta il tipo di sfondo su Colore
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Imposta il colore di sfondo
            odsPageBackground.Color = Color.LightBlue;

            // Imposta il tipo di grafica di sfondo
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Imposta la posizione della grafica di sfondo
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Imposta il percorso della grafica collegata (se presente)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Salva la cartella di lavoro
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


