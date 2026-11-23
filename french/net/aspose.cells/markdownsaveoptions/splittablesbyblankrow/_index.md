---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Indique si les lignes vides dans la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers Markdown. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers Markdown. La valeur par défaut est false.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple avec des lignes vides pour démontrer la division des tableaux
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Ajoutez une ligne vide (ligne 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // Créer une instance de MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Affichez la valeur par défaut de SplitTablesByBlankRow
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Définissez SplitTablesByBlankRow sur true pour diviser les tableaux par des lignes vides
                saveOptions.SplitTablesByBlankRow = true;

                // Afficher la valeur mise à jour
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Enregistrez le classeur au format markdown avec la division des tableaux activée
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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


