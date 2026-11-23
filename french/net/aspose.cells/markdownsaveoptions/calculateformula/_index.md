---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown.

```csharp
public bool CalculateFormula { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des formules
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Créer une instance de MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Afficher la valeur par défaut de CalculateFormula
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Définir CalculateFormula sur true pour calculer les formules avant l'enregistrement
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Enregistrer le classeur avec le calcul des formules activé
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Définir CalculateFormula sur false pour enregistrer les formules telles quelles
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Enregistrer le classeur avec le calcul des formules désactivé
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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


