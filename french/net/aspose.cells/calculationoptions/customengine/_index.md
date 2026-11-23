---
title: "CalculationOptions.CustomEngine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells"
type: docs
url: /fr/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCustomEngineDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Définir la formule HYPERLINK dans la cellule A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // Créer un moteur personnalisé qui traite la fonction HYPERLINK
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Définir les options de calcul avec un moteur personnalisé
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Calculez les formules avec le moteur personnalisé
            wb.CalculateFormula(options);
            
            Console.WriteLine("Custom engine invoked: " + customEngine.Invoked);
        }
    }

    public class CustomEngineForHyperlink : AbstractCalculationEngine
    {
        public bool Invoked { get; private set; }
        private readonly bool _shouldProcess;

        public CustomEngineForHyperlink(bool shouldProcess)
        {
            _shouldProcess = shouldProcess;
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "HYPERLINK" && _shouldProcess)
            {
                Invoked = true;
                data.CalculatedValue = "[Custom Processed] " + data.GetParamText(1);
            }
            // N'appelez pas base.Calculate() car il est abstrait
            // Laissez simplement le calcul par défaut s'exécuter pour les autres fonctions
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


