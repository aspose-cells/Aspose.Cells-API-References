---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique si elle calcule toutes les formules à chaque fois qu'un calcul est déclenché"
type: docs
url: /fr/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Indique s'il calcule toutes les formules à chaque déclenchement d'un calcul.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Remarques

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des raisons de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule du classeur automatiquement, quel que soit la valeur définie pour cette propriété.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres de formule
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Démontrer la propriété ForceFullCalculation
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Ajoutez des données d'exemple et une formule
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calculer les formules avec le paramètre ForceFullCalculation
            workbook.CalculateFormula();

            // Afficher le résultat
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Enregistrez le classeur
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


