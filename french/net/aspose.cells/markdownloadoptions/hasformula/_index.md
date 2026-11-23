---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownLoadOptions. Indique si le texte est une formule s'il commence par"
type: docs
url: /fr/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Indique si le texte est une formule lorsqu'il commence par "=".

```csharp
public bool HasFormula { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Afficher la valeur par défaut de HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Définir HasFormula sur true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Définir HasFormula sur false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Créer un workbook avec du contenu markdown d'exemple
                Workbook workbook = new Workbook();

                // Enregistrer le workbook pour démontrer que les options peuvent être utilisées
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


