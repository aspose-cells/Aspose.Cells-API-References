---
title: "Workbook.ChangePalette"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Cambia la tavolozza per il foglio di calcolo nell'indice specificato"
type: docs
url: /it/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

Modifica la tavolozza per il foglio di calcolo nell'indice specificato.

```csharp
public void ChangePalette(Color color, int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | Struttura Color. |
| indice | Int32 | Indice della tavolozza, 0 - 55. |

### Osservazioni

La tavolozza ha 56 voci, ciascuna rappresentata da un valore RGB.

Se imposti un colore che non è nella tavolozza, non avrà effetto.

Quindi, se vuoi impostare un colore personalizzato, per favore cambia prima la tavolozza.

Di seguito è la tavolozza di colori standard.

| **Color** | **Red** | **Verde** | **Blu** |
| --- | --- | --- | --- |
| Nero | 0 | 0 | 0 |
| Bianco | 255 | 255 | 255 |
| Rosso | 255 | 0 | 0 |
| Lime | 0 | 255 | 0 |
| Blu | 0 | 0 | 255 |
| Giallo | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Ciano | 0 | 255 | 255 |
| Marrone | 128 | 0 | 0 |
| Verde | 0 | 128 | 0 |
| Blu navy | 0 | 0 | 128 |
| Oliva | 128 | 128 | 0 |
| Viola | 128 | 0 | 128 |
| Verde acqua | 0 | 128 | 128 |
| Argento | 192 | 192 | 192 |
| Grigio | 128 | 128 | 128 |
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

### Esempi

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
            // Crea un'istanza di cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Cambia il colore della tavolozza all'indice 55
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile con il colore della tavolozza modificato
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


