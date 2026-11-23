---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les en-têtes de lignes et de colonnes des feuilles sont exportés lors de l’enregistrement en fichiers HTML"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille est activée lors de l'enregistrement en fichiers HTML.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir ExportRowColumnHeadings sur false (la valeur par défaut est true).
            saveOptions.ExportRowColumnHeadings = false;

            // Enregistrez le classeur avec les en-têtes désactivés
            workbook.Save("output_without_headings.html", saveOptions);

            // Activez maintenant les en-têtes et enregistrez à nouveau
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


