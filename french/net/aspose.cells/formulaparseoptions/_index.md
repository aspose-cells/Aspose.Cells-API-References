---
title: "Classe FormulaParseOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FormulaParseOptions. Représente les options lors de l'analyse d'une formule"
type: docs
url: /fr/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Représente les options lors de l'analyse d'une formule.

```csharp
public class FormulaParseOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true (si la fonction définie par l'utilisateur correspond à un complément dans les liens externes existants, alors il est considéré comme le complément). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Définition pour l'analyse des fonctions personnalisées. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Indique si la formule est formatée selon la locale. La valeur par défaut est false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Indique s'il faut analyser la formule donnée. La valeur par défaut est true. Si elle est false, la chaîne de formule fournie sera conservée telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour l'analyser ou que les données de formule analysée soient requises par d'autres opérations telles que le calcul des formules. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Indique si la formule utilise le style de référence R1C1. La valeur par défaut est false. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Ajouter une formule à une cellule en utilisant les options
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Enregistrez le classeur
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


