---
title: "ShapeCollection.AddTextEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Inserisce un oggetto WordArt"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Inserisce un oggetto WordArt.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| effetto | MsoPresetTextEffect | Il tipo di effetto di testo predefinito mso. |
| testo | String | Il testo WordArt. |
| fontName | String | Il nome del carattere. |
| dimensione | Int32 | La dimensione del carattere |
| fontBold | Booleano | Indica se il carattere è in grassetto. |
| fontItalic | Booleano | Indica se il carattere è in corsivo. |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della forma dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza della shape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza della forma, in unità di pixel. |

### Valore di ritorno

Restituisce un oggetto Shape che rappresenta il nuovo oggetto WordArt.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


