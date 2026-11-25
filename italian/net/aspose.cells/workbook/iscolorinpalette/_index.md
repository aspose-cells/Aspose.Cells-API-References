---
title: "Workbook.IsColorInPalette"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Verifica se un colore è nella tavolozza per il foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Verifica se un colore è nella tavolozza per il foglio di calcolo.

```csharp
public bool IsColorInPalette(Color color)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | Struttura Color. |

### Valore di ritorno

Restituisce true se questo colore è nella tavolozza. Altrimenti, restituisce false

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Verifica se il colore standard esiste nella tavolozza
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Verifica se il colore personalizzato esiste nella tavolozza
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Ottieni il colore corrispondente dalla tavolozza
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


