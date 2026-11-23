---
title: "WorkbookRender.PageCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookRender. Obtient le nombre total de pages du classeur"
type: docs
url: /fr/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Obtient le nombre total de pages du classeur.

```csharp
public int PageCount { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Ajouter une deuxième feuille de calcul
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Créer des options de rendu et le rendu du classeur
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Démontrer l'utilisation de PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Rendre chaque page en image
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


