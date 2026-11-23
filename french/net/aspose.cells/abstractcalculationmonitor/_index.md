---
title: "Classe AbstractCalculationMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AbstractCalculationMonitor. Moniteur permettant à l'utilisateur de suivre la progression du calcul des formules"
type: docs
url: /fr/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Permet à l'utilisateur de suivre la progression du calcul de la formule.

```csharp
public abstract class AbstractCalculationMonitor
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Obtient la nouvelle valeur calculée de la cellule. Ne doit être utilisé que dans [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Obtient l'ancienne valeur de la cellule calculée. Ne doit être utilisé que dans [`BeforeCalculate`](./beforecalculate/) et [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Indique si la valeur de la cellule a été modifiée après le calcul. Ne doit être utilisé que dans [`AfterCalculate`](./aftercalculate/). |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implémentez cette méthode pour effectuer des opérations après le calcul d'une cellule. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implémentez cette méthode pour effectuer des opérations avant le calcul d'une cellule. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implémentez cette méthode pour effectuer les opérations lors du calcul des formules avec des références circulaires. |

### Exemples

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Implémentation personnalisée de AbstractCalculationMonitor
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Créez une instance de CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Définissez les options de calcul
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Calculez les formules avec le moniteur personnalisé
            workbook.CalculateFormula(options);

            // Enregistrez le classeur
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


