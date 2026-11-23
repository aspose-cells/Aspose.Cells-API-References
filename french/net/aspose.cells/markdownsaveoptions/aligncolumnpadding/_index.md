---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Indique si l'alignement des colonnes est activé pour les tables Markdown générées. Lorsqu'il est activé, les colonnes sont alignées en remplissant le contenu des cellules avec le caractère spécifié, généralement des espaces. Définir à 0 pour désactiver l'alignement des colonnes par défaut"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Indique si l'alignement des colonnes est activé pour les tables Markdown générées. Lorsqu'il est activé, les colonnes sont alignées en remplissant le contenu des cellules avec le caractère spécifié (généralement ' ' pour les espaces). Définissez à '\\0' pour désactiver l'alignement des colonnes (par défaut).

```csharp
public char AlignColumnPadding { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour démontrer l'alignement des colonnes
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Créer une instance de MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Afficher la valeur par défaut d'AlignColumnPadding
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Définir AlignColumnPadding au caractère espace pour l'alignement des colonnes
                saveOptions.AlignColumnPadding = ' ';

                // Afficher la valeur mise à jour
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Enregistrer le classeur au format markdown avec alignement des colonnes
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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


