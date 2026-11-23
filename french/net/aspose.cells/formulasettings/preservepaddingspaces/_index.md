---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique s'il faut conserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Indique s'il faut conserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de la récupération et de la définition des formules. La valeur par défaut est false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Remarques

En général, ces espaces et sauts de ligne ne servent qu'à l'affichage ; les conserver ou non n'affecte pas le résultat calculé. Pour des raisons de performance, s'il n'y a aucune exigence particulière, il vaut mieux ne pas les conserver lors du traitement des formules.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la formule avec des espaces de remplissage
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Comportement par défaut (PreservePaddingSpaces est true)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Modifier le paramètre pour supprimer les espaces de remplissage
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Enregistrez le classeur
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


