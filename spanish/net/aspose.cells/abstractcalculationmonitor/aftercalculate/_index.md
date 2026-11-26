---
title: "AbstractCalculationMonitor.AfterCalculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractCalculationMonitor. Implemente este método para realizar operaciones después de que se haya calculado una celda"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/aftercalculate/
---
## AbstractCalculationMonitor.AfterCalculate method

Implementa este método para realizar acciones después de que se haya calculado una celda.

```csharp
public virtual void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | Índice de la hoja a la que pertenece la celda. |
| rowIndex | Int32 | Índice de fila de la celda |
| colIndex | Int32 | Índice de columna de la celda |

### Ejemplos

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

            // Configurar fórmulas de ejemplo
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

### Ver también

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


