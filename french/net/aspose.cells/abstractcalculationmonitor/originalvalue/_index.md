---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractCalculationMonitor. Obtient l'ancienne valeur de la cellule calculée. Ne doit être utilisée que dans BeforeCalculate et AfterCalculate"
type: docs
url: /fr/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Obtient l'ancienne valeur de la cellule calculée. Ne doit être utilisée que dans [`BeforeCalculate`](../beforecalculate/) et [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor1 : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyOriginalValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la valeur initiale
            worksheet.Cells["A1"].PutValue(10);
            
            // Ajouter une formule qui modifiera la valeur
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Définir le moniteur de calcul
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Recalculer les formules - cela déclenchera le moniteur
            workbook.CalculateFormula(options);
            
            // Modifier la valeur originale pour démontrer le moniteur
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


