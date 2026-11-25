---
title: "Enum OdsPageBackgroundType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundType enum. Rappresenta il tipo di sfondo della pagina di ods"
type: docs
url: /it/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

Rappresenta il tipo di sfondo della pagina di ods.

```csharp
public enum OdsPageBackgroundType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuno sfondo. |
| Color | `1` | Formatta lo sfondo con colore. |
| Graphic | `2` | Formatta lo sfondo con immagine. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi al PageSetup del foglio di lavoro
            PageSetup pageSetup = worksheet.PageSetup;

            // Accedi alla proprietà ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Imposta il tipo di sfondo su Colore
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Imposta il colore di sfondo
            odsPageBackground.Color = Color.LightBlue;

            // Salva la cartella di lavoro
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


