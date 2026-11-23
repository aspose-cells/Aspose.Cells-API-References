---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractCalculationEngine. Ignore le calcul pour toute la formule qui fait référence à la fonction actuellement évaluée"
type: docs
url: /fr/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Ignore le calcul de toute la formule qui fait référence à la fonction actuellement évaluée.

```csharp
public void SkipCalculation()
```

### Remarques

Cette méthode peut être invoquée dans l'implémentation de [`Calculate`](../calculate/) pour ignorer le calcul de toute la formule et la valeur originale de la formule sera conservée sans modification.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Créer un moteur de calcul personnalisé
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Calculer le classeur qui déclenchera notre moteur personnalisé
                workbook.CalculateFormula(options);

                // Afficher le résultat (devrait être ignoré)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Enregistrez le classeur
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // Ignorer le calcul pour cette formule
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


