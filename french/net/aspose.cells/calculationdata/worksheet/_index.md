---
title: "CalculationData.Worksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationData. Obtient l'objet Worksheet où se trouve la fonction"
type: docs
url: /fr/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Obtient l'objet Worksheet où se trouve la fonction.

```csharp
public Worksheet Worksheet { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter des données pour rendre l’exemple significatif
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Créer des options de calcul avec un moteur personnalisé
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Calculer les formules avec des options
                workbook.CalculateFormula(options);

                // Afficher le résultat
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Enregistrer le résultat
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Accéder à la propriété Worksheet en lecture seule
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


