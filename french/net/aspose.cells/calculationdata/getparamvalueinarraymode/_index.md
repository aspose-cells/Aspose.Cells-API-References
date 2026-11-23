---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CalculationData. Obtient les valeurs du paramètre à un indice donné. Si le paramètre est une sorte d'expression qui doit être calculée, il sera calculé en mode tableau"
type: docs
url: /fr/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Obtient la ou les valeurs du paramètre à un index donné. Si le paramètre est une sorte d'expression qui doit être calculée, elle sera calculée en mode tableau.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice du paramètre (à partir de 0) |
| maxRowCount | Int32 | La limite du nombre de lignes pour le tableau retourné. Si elle est non positive ou supérieure au nombre réel de lignes, alors le nombre réel de lignes sera utilisé. |
| maxColumnCount | Int32 | La limite du nombre de colonnes pour le tableau retourné. Si elle est non positive ou supérieure au nombre réel de lignes, alors le nombre réel de colonnes sera utilisé. |

### Valeur de retour

Un tableau qui contient tous les éléments représentés par le paramètre spécifié.

### Remarques

Pour une expression qui doit être calculée, en prenant A:A+B:B comme exemple : en mode valeur, elle sera calculée en une seule valeur selon la base de la cellule actuelle. Mais en mode tableau, toutes les valeurs de A1+B1, A2+B2, A3+B3, … seront calculées et utilisées pour construire le tableau retourné. Et pour ce type de situation, il est préférable de spécifier la limite du nombre de lignes/colonnes (par exemple selon [`MaxDataRow`](../../cells/maxdatarow/) et [`MaxDataColumn`](../../cells/maxdatacolumn/)), sinon le grand tableau retourné peut augmenter le coût mémoire avec une grande quantité de données inutiles.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le contexte
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Créer des options de calcul avec un moteur personnalisé
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Appelez GetParamValueInArrayMode avec des paramètres réalistes
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


