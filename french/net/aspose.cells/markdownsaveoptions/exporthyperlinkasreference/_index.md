---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Indique s'il faut exporter les hyperliens en utilisant des définitions de référence au lieu du format en ligne. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Indique s'il faut exporter les hyperliens en utilisant des définitions de référence au lieu du format en ligne. La valeur par défaut est false.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Mettez un texte d'exemple dans une cellule
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Ajoutez un hyperlien à la cellule (A1)
            // Paramètres : firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Initialisez les options d'enregistrement Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Accédez directement à la propriété ExportHyperlinkAsReference (lecture‑seule dans cette démo)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Enregistrez le classeur au format markdown ; la propriété (si true) affectera la façon dont les hyperliens sont exportés
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


