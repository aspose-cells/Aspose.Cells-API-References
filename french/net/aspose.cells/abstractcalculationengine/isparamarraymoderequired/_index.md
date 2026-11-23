---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractCalculationEngine. Indique si ce moteur nécessite que le paramètre soit calculé en mode tableau. La valeur par défaut est false. Si GetParamValueInArrayMode est requis lors du calcul de fonctions personnalisées et que l'utilisateur n'a pas mis à jour la définition de celles-ci via UpdateCustomFunctionDefinition, cette propriété doit être définie sur true."
type: docs
url: /fr/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Indique si ce moteur nécessite que le paramètre soit calculé en mode tableau. La valeur par défaut est false. Si [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) est requis lors du calcul de fonctions personnalisées et que l'utilisateur n'a pas mis à jour la définition de celles-ci (par [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)), cette propriété doit être définie sur true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Remarques

Si ce moteur de calcul personnalisé nécessite que le paramètre soit calculé en mode tableau, davantage de piles seront nécessaires pour mettre en cache l'arbre des paramètres et la méthode Calculate() pourra être appelée de manière récursive pour calculer la valeur du paramètre. Pour des raisons de performance, veuillez laisser cette propriété à la valeur par défaut (false) s'il n'y a aucune exigence particulière.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamArrayModeRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomCalculationEngine engine = new CustomCalculationEngine();
            Console.WriteLine("IsParamArrayModeRequired: " + engine.IsParamArrayModeRequired);

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].Formula = "=SUMARRAY(A1,A2)";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            Console.WriteLine("SUMARRAY result: " + worksheet.Cells["A3"].Value);

            workbook.Save("IsParamArrayModeRequiredDemo.xlsx");
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override bool IsParamArrayModeRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUMARRAY")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(i);

                    double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));

                    sum += param1;
                }
                data.CalculatedValue = sum;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            return false;
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


