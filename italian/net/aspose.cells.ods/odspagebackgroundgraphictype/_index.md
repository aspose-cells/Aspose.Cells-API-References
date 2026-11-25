---
title: "Enum OdsPageBackgroundGraphicType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Rappresenta il tipo di sfondo della pagina di formattazione con immagine"
type: docs
url: /it/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Rappresenta il tipo di formattazione dello sfondo della pagina con immagine.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Position | `0` | Imposta l'immagine in una posizione specifica. |
| Area | `1` | Allunga l'immagine. |
| Tile | `2` | Ripeti e ripeti l'immagine. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi al PageSetup del foglio di lavoro
            PageSetup pageSetup = worksheet.PageSetup;

            // Accedi a ODSPageBackground del PageSetup
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Imposta il colore di sfondo
            odsPageBackground.Color = Color.LightBlue;

            // Imposta il tipo di grafica di sfondo su Tile
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Imposta il percorso della grafica collegata (supponendo che l'immagine sia nella stessa directory dell'eseguibile)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Salva la cartella di lavoro
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


