---
title: "SheetSet.All"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SheetSet. Obtient un ensemble contenant toutes les feuilles du classeur dans leur ordre d'origine"
type: docs
url: /fr/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Obtient un ensemble avec toutes les feuilles du classeur dans leur ordre d'origine.

```csharp
public static SheetSet All { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // Créer un classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Définissez des données d'exemple dans les deux feuilles
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Enregistrer toutes les feuilles au format markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### Voir aussi

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


