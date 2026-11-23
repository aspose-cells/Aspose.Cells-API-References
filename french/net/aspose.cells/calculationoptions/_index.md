---
title: "Classe CalculationOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CalculationOptions. Représente les options de calcul"
type: docs
url: /fr/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Représente les options de calcul.

```csharp
public class CalculationOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | Le moniteur permettant à l'utilisateur de suivre la progression du calcul des formules. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Spécifie l'encodage utilisé pour encoder/décoder les caractères lors du calcul des formules. Pour des fonctions telles que CHAR, CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé par ces fonctions pour obtenir le résultat attendu. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. L'erreur peut être une fonction non prise en charge, des liens externes, etc. La valeur par défaut est true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Spécifie les sources de données pour les liens externes utilisés dans les formules. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Spécifie la stratégie de traitement de la précision du calcul. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. La valeur par défaut est true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Indique si les formules de tableau dynamique doivent être actualisées avant de calculer les formules. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Indique si l'utilisateur a explicitement spécifié le comportement d'actualisation des formules de tableau dynamique avant de calculer les formules spécifiées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Créez une instance de CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // Optionnellement, vous pouvez définir un moteur de calcul personnalisé ou un moniteur
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Calculez les formules dans le classeur avec les options spécifiées
            workbook.CalculateFormula(calcOptions);

            // Enregistrez le classeur
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Exemple de moteur de calcul personnalisé (si nécessaire)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Logique de calcul personnalisée
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Exemple de logique de fonction personnalisée
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Traitez le paramètre ici
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Exemple de moniteur de calcul personnalisé (si nécessaire)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logique avant le calcul
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logique après le calcul
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Gérer les références circulaires
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


