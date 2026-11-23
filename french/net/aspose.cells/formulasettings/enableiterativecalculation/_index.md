---
title: "FormulaSettings.EnableIterativeCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique s'il faut activer le calcul itératif pour résoudre les références circulaires"
type: docs
url: /fr/net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Indique s'il faut activer le calcul itératif pour résoudre les références circulaires.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurer une référence circulaire pour la démonstration
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Activer le calcul itératif avec le nombre maximal d'itérations
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Calculer les formules
            workbook.CalculateFormula();
            
            // Afficher les résultats
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


