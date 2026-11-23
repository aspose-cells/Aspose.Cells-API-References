---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Indique si les formules de tableau dynamique doivent être actualisées avant le calcul des formules"
type: docs
url: /fr/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Indique si les formules de tableau dynamique doivent être actualisées avant de calculer les formules.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Remarques

Si cette propriété a été spécifiée explicitement, la valeur indiquée sera utilisée pour déterminer s'il faut actualiser les formules de tableau dynamique. Sinon ( [`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) est faux ), la valeur par défaut dépend du type de formules à calculer : pour le calcul des formules du classeur, comme [`CalculateFormula`](../../workbook/calculateformula/), cette propriété sera considérée comme vraie. Dans les autres cas, comme [`Calculate`](../../cell/calculate/) ou [`CalculateFormula`](../../worksheet/calculateformula/), cette propriété sera considérée comme fausse.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une formule de tableau dynamique pour démontrer la fonctionnalité
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // Créer une instance de CalculationOptions
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Afficher la valeur par défaut de RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Définir la propriété sur true pour actualiser les formules de tableau dynamique
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Calculer les formules avec les options spécifiées
                workbook.CalculateFormula(options);

                // Afficher le résultat calculé
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Enregistrez le classeur
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


