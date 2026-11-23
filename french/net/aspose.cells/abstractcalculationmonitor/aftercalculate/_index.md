---
title: "AbstractCalculationMonitor.AfterCalculate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractCalculationMonitor. Implémentez cette méthode pour effectuer des opérations après qu'une cellule a été calculée"
type: docs
url: /fr/net/aspose.cells/abstractcalculationmonitor/aftercalculate/
---
## AbstractCalculationMonitor.AfterCalculate method

Implémentez cette méthode pour effectuer des opérations après le calcul d'une cellule.

```csharp
public virtual void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index de la feuille à laquelle la cellule appartient. |
| rowIndex | Int32 | Index de ligne de la cellule |
| colIndex | Int32 | Indice de colonne de la cellule |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationMonitorMethodAfterCalculateWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurer des formules d'exemple
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["B1"].Formula = "=NOW()"; // Volatile function

            CalculationOptions options = new CalculationOptions();
            var monitor = new CalculationMonitor();
            options.CalculationMonitor = monitor;

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check cell values and console output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("AfterCalculateDemo.xlsx");
        }


        private class CalculationMonitor : AbstractCalculationMonitor
        {
            public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
            {
                Console.WriteLine($"Calculated cell (Sheet {sheetIndex}): Row {rowIndex}, Column {colIndex}");
                Console.WriteLine($"Value changed: {ValueChanged}, Original: {OriginalValue}, New: {CalculatedValue}");
                Console.WriteLine("----------------------------------");
            }
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


