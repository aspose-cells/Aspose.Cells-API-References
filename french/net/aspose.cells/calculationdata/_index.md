---
title: "Classe CalculationData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CalculationData. Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres ...etc"
type: docs
url: /fr/net/aspose.cells/calculationdata/
---
## CalculationData class

Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres, ...etc.

```csharp
public class CalculationData
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Obtient ou définit la valeur calculée pour cette fonction. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Obtient l'objet Cell où se trouve la fonction. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Obtient l'index de colonne de la cellule où se trouve la fonction. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Obtient l'index de ligne de la cellule où se trouve la fonction. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Obtient le nom de la fonction à calculer. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Obtient le nombre de paramètres |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Obtient l'objet Workbook où se trouve la fonction. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Obtient l'objet Worksheet où se trouve la fonction. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Obtient le texte littéral du paramètre à l'index donné. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Obtient l'objet valeur représentée du paramètre à un index donné. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Obtient la ou les valeurs du paramètre à un index donné. Si le paramètre est une sorte d'expression qui doit être calculée, elle sera calculée en mode tableau. |

### Remarques

Tous les objets fournis par cette classe sont uniquement destinés à la lecture. L'utilisateur ne doit pas modifier les données du Workbook pendant le processus de calcul de formule, sinon un résultat inattendu ou une Exception peut survenir.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Préparez un classeur et une feuille de calcul simples
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Placez quelques valeurs qui seront utilisées comme paramètres dans une fonction personnalisée
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Définissez une formule qui invoque la fonction personnalisée
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Configurer les options de calcul pour utiliser un moteur personnalisé
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Effectuer le calcul – le moteur personnalisé recevra une instance de CalculationData
                workbook.CalculateFormula(options);

                // Afficher le résultat de la fonction personnalisée
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Enregistrer le classeur pour plus de complétude
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Moteur de calcul personnalisé qui démontre l'accès aux membres de CalculationData
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Assurez‑vous que nous gérons la fonction personnalisée attendue
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Récupérer les valeurs des paramètres (elles sont renvoyées sous forme d'objets)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Convertir les paramètres en double pour le calcul
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Attribuer le résultat calculé
                    data.CalculatedValue = result;

                    // Démontrer la lecture des propriétés en lecture seule
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


