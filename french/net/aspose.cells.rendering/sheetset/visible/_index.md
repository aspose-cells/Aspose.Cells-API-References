---
title: "SheetSet.Visible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SheetSet. Obtient un ensemble contenant les feuilles visibles du classeur dans leur ordre d'origine"
type: docs
url: /fr/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Obtient un ensemble avec les feuilles visibles du classeur dans leur ordre d'origine.

```csharp
public static SheetSet Visible { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Masquer la deuxième feuille de calcul
            workbook.Worksheets[1].IsVisible = false;

            // Configurer les options d’enregistrement pour n’exporter que les feuilles visibles
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Enregistrer le classeur (seule la feuille visible sera exportée)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### Voir aussi

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


