---
title: "AbstractCalculationEngine.ProcessBuiltInFunctions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractCalculationEngine. Indique si les fonctions intégrées prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/abstractcalculationengine/processbuiltinfunctions/
---
## AbstractCalculationEngine.ProcessBuiltInFunctions property

Indique si les fonctions intégrées prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation. La valeur par défaut est false.

```csharp
public virtual bool ProcessBuiltInFunctions { get; }
```

### Remarques

Si l'utilisateur doit modifier la logique de calcul de certaines fonctions intégrées, cette propriété doit être définie sur true. Sinon, veuillez laisser cette propriété sur false pour des raisons de performance.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyProcessBuiltInFunctionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir les données de test
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Créer des moteurs de calcul personnalisés avec des valeurs différentes de ProcessBuiltInFunctions
            CustomEngine engineProcessEnabled = new CustomEngine(true);
            CustomEngine engineProcessDisabled = new CustomEngine(false);

            // Afficher les valeurs des propriétés
            Console.WriteLine("Engine1 ProcessBuiltInFunctions: " + engineProcessEnabled.ProcessBuiltInFunctions);
            Console.WriteLine("Engine2 ProcessBuiltInFunctions: " + engineProcessDisabled.ProcessBuiltInFunctions);

            // Calculer avec le moteur personnalisé (ProcessBuiltInFunctions = true)
            CalculationOptions optionsEnabled = new CalculationOptions { CustomEngine = engineProcessEnabled };
            workbook.CalculateFormula(optionsEnabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=true: " + worksheet.Cells["A4"].Value);

            // Calculer avec le moteur personnalisé (ProcessBuiltInFunctions = false)
            CalculationOptions optionsDisabled = new CalculationOptions { CustomEngine = engineProcessDisabled };
            workbook.CalculateFormula(optionsDisabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=false: " + worksheet.Cells["A4"].Value);

            workbook.Save("ProcessBuiltInFunctionsDemo.xlsx");
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        private readonly bool _processBuiltIn;

        public CustomEngine(bool processBuiltIn)
        {
            _processBuiltIn = processBuiltIn;
        }

        public override bool ProcessBuiltInFunctions => _processBuiltIn;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("SUM", StringComparison.OrdinalIgnoreCase) && ProcessBuiltInFunctions)
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object param = data.GetParamValue(i);
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);

                    for (int r = paramArea1.StartRow; r <= paramArea1.EndRow; r++)
                    {
                        for (int c = paramArea1.StartColumn; c <= paramArea1.EndColumn; c++)
                        {
                            object cellValue = paramArea1.GetValue(r, c);
                            sum += Convert.ToDouble(cellValue);
                        }
                    }
                    
                }
                data.CalculatedValue = sum * 2; // Custom SUM implementation doubles the result
            }
            // Les autres fonctions sont gérées par le moteur par défaut
        }

        public override bool ForceRecalculate(string functionName) => false;
    }
}
```

### Voir aussi

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


