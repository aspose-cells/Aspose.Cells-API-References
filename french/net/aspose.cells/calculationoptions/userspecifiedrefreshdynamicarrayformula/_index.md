---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Indique si l'utilisateur a explicitement spécifié le comportement du rafraîchissement des formules de tableau dynamique avant de calculer les formules spécifiées"
type: docs
url: /fr/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Indique si l'utilisateur a explicitement spécifié le comportement d'actualisation des formules de tableau dynamique avant de calculer les formules spécifiées.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer une instance de CalculationOptions
                CalculationOptions options = new CalculationOptions();

                // Afficher la valeur actuelle de la propriété UserSpecifiedRefreshDynamicArrayFormula
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Enregistrer le résultat
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


