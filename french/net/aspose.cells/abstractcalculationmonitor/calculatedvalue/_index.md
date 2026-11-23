---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractCalculationMonitor. Obtient la nouvelle valeur calculée de la cellule. Ne doit être utilisée que dans AfterCalculate"
type: docs
url: /fr/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Obtient la nouvelle valeur calculée de la cellule. Ne doit être utilisée que dans [`AfterCalculate`](../aftercalculate/).

```csharp
public object CalculatedValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurer la chaîne de calcul
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Créer et attacher le moniteur
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Déclencher le calcul qui invoquera notre moniteur
            workbook.CalculateFormula(options);

            // Modifier une valeur pour déclencher la notification de changement de valeur
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


