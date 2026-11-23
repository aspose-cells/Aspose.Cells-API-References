---
title: "AutoFitterOptions.ForRendering"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFitterOptions. Indique si l'ajustement est destiné au rendu"
type: docs
url: /fr/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Indique si l'ajustement est destiné au rendu.

```csharp
public bool ForRendering { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple avec un texte long
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // Créer AutoFitterOptions et définir ForRendering sur true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Ajuster automatiquement la ligne en tenant compte du rendu
            worksheet.AutoFitRows(0, 0, options);

            // Afficher la hauteur de ligne résultante en pixels
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


