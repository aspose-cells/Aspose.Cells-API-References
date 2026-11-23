---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractCalculationMonitor. Implémentez cette méthode pour effectuer des opérations lors du calcul de formules avec des références circulaires"
type: docs
url: /fr/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Implémentez cette méthode pour effectuer les opérations lors du calcul des formules avec des références circulaires.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator avec des éléments [`CalculationCell`](../../calculationcell/) représentant les cellules qui dépendent de références circulaires. |

### Valeur de retour

Indique si le moteur de formules doit calculer ces cellules en boucle après cet appel. True pour permettre au moteur de formules de continuer le calcul pour elles. False pour que le moteur de formules se contente de marquer ces cellules comme Calculated.

### Remarques

Dans l'implémentation, l'utilisateur peut également définir la valeur attendue comme résultat calculé pour une partie ou la totalité de ces cellules afin que le moteur de formules ne les calcule pas de manière récursive.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un scénario de référence circulaire
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


