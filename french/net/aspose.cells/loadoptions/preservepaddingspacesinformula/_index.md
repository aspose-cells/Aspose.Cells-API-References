---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Indique s’il faut conserver les espaces et sauts de ligne qui sont insérés entre les jetons de formule lors de la lecture et de l’écriture des formules. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Indique s'il faut conserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de l'obtention et de la définition des formules. La valeur par défaut est false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Remarques

Après avoir chargé le classeur à partir du fichier modèle avec cette option, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) sera défini sur la même valeur que cette propriété.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Activer la conservation des espaces de remplissage dans les formules
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // Accéder à la première feuille de calcul et définir une formule avec des espaces de remplissage
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Enregistrer et recharger le classeur avec l’option PreservePaddingSpacesInFormula
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Vérifier que la formule a conservé les espaces après le rechargement
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


