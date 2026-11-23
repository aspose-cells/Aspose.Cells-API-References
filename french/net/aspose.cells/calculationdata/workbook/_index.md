---
title: "CalculationData.Workbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationData. Obtient l'objet Workbook où la fonction se trouve"
type: docs
url: /fr/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Obtient l'objet Workbook où se trouve la fonction.

```csharp
public Workbook Workbook { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple et une formule
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Créer des options de calcul et enregistrer le moteur de calcul personnalisé
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Déclencher le calcul avec des options pour démontrer l'utilisation de la propriété Workbook
            workbook.CalculateFormula(options);

            // Afficher le résultat du calcul
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Enregistrer le résultat
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // Accéder à la propriété Workbook depuis CalculationData
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Démontrer l'utilisation de Workbook pour manipuler les données
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Définir le résultat calculé
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


