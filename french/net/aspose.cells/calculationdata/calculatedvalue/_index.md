---
title: "CalculationData.CalculatedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationData. Obtient ou définit la valeur calculée pour cette fonction"
type: docs
url: /fr/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Obtient ou définit la valeur calculée pour cette fonction.

```csharp
public object CalculatedValue { get; set; }
```

### Remarques

L'utilisateur doit définir cette propriété dans son moteur de calcul personnalisé pour les fonctions prises en charge par le moteur, et la valeur définie sera renvoyée lors de la lecture ultérieure de cette propriété. La valeur définie peut être de types possibles de [`Value`](../../cell/value/), ou un tableau de ce type de valeurs, ou une Range, Name, ReferredArea. Lire cette propriété avant d'y avoir assigné une valeur entraînera le calcul de la fonction par le moteur de calcul par défaut d'Aspose.Cells, puis la valeur calculée sera renvoyée (généralement #NAME? pour les fonctions définies par l'utilisateur).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Créer des options de calcul avec un moteur personnalisé
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Calculer les formules avec des options
            workbook.CalculateFormula(options);

            // Obtenir la valeur calculée
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
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

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


