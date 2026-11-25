---
title: "Enum PresetWordArtStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.PresetWordArtStyle. Rappresenta gli stili WordArt predefiniti"
type: docs
url: /it/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Rappresenta gli stili WordArt predefiniti.

```csharp
public enum PresetWordArtStyle
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| WordArtStyle1 | `1` | Riempimento - Nero, Testo 1, Ombra |
| WordArtStyle2 | `2` | Riempimento - Blu, Accento 1, Ombra |
| WordArtStyle3 | `3` | Riempimento - Arancione, Accento 2, Contorno - Accento 2 |
| WordArtStyle4 | `4` | Riempimento - Bianco, Contorno - Accento 1, Ombra |
| WordArtStyle5 | `5` | Riempimento - Oro, Accento 4, Smussatura morbida |
| WordArtStyle6 | `6` | Riempimento gradiente - Grigio |
| WordArtStyle7 | `7` | Riempimento gradiente - Blu, Accento 1, Riflesso |
| WordArtStyle8 | `8` | Riempimento gradiente - Oro, Accento 4, Contorno - Accento 4 |
| WordArtStyle9 | `9` | Riempimento - Bianco, Contorno - Accento 1, Bagliore - Accento 1 |
| WordArtStyle10 | `10` | Riempimento - Grigio-50%, Accento 3, Smussatura netta |
| WordArtStyle11 | `11` | Riempimento - Nero, Testo 1, Contorno - Sfondo 1, Ombra rigida - Sfondo 1 |
| WordArtStyle12 | `12` | Riempimento - Nero, Testo 1, Contorno - Sfondo 1, Ombra rigida - Accento 1 |
| WordArtStyle13 | `13` | Riempimento - Blu, Accento 1, Contorno - Sfondo 1, Ombra rigida - Accento 1 |
| WordArtStyle14 | `14` | Riempimento - Bianco, Contorno - Accento 2, Ombra rigida - Accento 2 |
| WordArtStyle15 | `15` | Riempimento - Grigio-25%, Sfondo 2, Ombra interna |
| WordArtStyle16 | `16` | Riempimento a trama - Bianco, Testo 2, Diagonale ascendente scura, Ombra |
| WordArtStyle17 | `17` | Riempimento a trama - Grigio-50%, Accento 3, Orizzontale stretto, Ombra interna |
| WordArtStyle18 | `18` | Riempimento - Blu, Accento 1, 50%, Ombra rigida - Accento 1 |
| WordArtStyle19 | `19` | Riempimento a trama - Blu, Accento 1, Diagonale discendente chiara, Contorno - Accento 1 |
| WordArtStyle20 | `20` | Riempimento a trama - Blu-grigio, Testo 2, Diagonale ascendente scura, Ombra rigida - Testo 2 |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla raccolta di forme del foglio di lavoro
            ShapeCollection shapes = worksheet.Shapes;
            
            // Aggiungi una forma WordArt con uno stile predefinito specifico
            // Parametri: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Salva la cartella di lavoro
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


