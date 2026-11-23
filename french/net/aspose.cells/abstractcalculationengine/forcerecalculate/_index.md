---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractCalculationEngine. Indique s'il faut forcer la fonction donnée à être recalculée à chaque fois lors du calcul des formules partagées"
type: docs
url: /fr/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Indique s'il faut forcer la fonction donnée à être recalculée à chaque fois lors du calcul des formules partagées.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| functionName | String | nom de la fonction. Généralement il s'agit du nom de la fonction personnalisée. Si [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) est vrai, alors les fonctions intégrées seront également vérifiées ici. |

### Valeur de retour

vrai si la fonction spécifiée doit toujours être recalculée.

### Remarques

Pour les formules partagées, plusieurs cellules partagent la même fonction. Si les paramètres de la fonction restent identiques pour ces cellules également, alors généralement cette fonction ne doit être calculée qu'une seule fois. Ainsi, pour des raisons de performance, nous ne calculons ce type de fonction qu'une fois également ( [`Calculate`](../calculate/) n'est appelé qu'une seule fois, au lieu d'être appelé de façon répétée pour chaque cellule). Cependant, dans l'implémentation personnalisée de l'utilisateur, il se peut que la fonction, en particulier la fonction personnalisée, doive être calculée différemment selon les cellules. Dans ce cas, l'utilisateur doit remplacer cette méthode pour qu'elle renvoie vrai pour la fonction. Et pour [`Calculate`](../calculate/), le [`CalculatedValue`](../../calculationdata/calculatedvalue/) fourni peut avoir été initialisé avec la valeur en cache du calcul précédent.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


