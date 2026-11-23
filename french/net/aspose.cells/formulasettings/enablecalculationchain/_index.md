---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique s'il faut activer la chaîne de calcul pour les formules. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Indique s'il faut activer la chaîne de calcul pour les formules. La valeur par défaut est false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Remarques

Lorsqu'il y a de nombreuses formules dans le classeur et que l'utilisateur doit les recalculer fréquemment en ne modifiant qu'une petite partie d'entre elles, activer la chaîne de calcul peut améliorer les performances. En revanche, si la chaîne est activée, le maintien du modèle de chaîne nécessite plus de mémoire et requiert un peu plus de temps CPU pour certaines autres opérations comme la modification de la valeur ou des formules d'une cellule. Après avoir changé cette propriété de false à true, la chaîne de calcul sera analysée et construite lors du premier calcul du classeur, de sorte que le temps requis pour le premier calcul peut être supérieur à un calcul normal sans chaîne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des formules d'exemple
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Désactiver la chaîne de calcul
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Calculer les formules
            workbook.CalculateFormula();
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


