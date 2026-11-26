---
title: "Clase AbstractCalculationMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AbstractCalculationMonitor. Monitor para que el usuario siga el progreso del cálculo de la fórmula"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Monitorea para que el usuario siga el progreso del cálculo de la fórmula.

```csharp
public abstract class AbstractCalculationMonitor
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Obtiene el valor recién calculado de la celda. Debe usarse solo en [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Obtiene el valor anterior de la celda calculada. Debe usarse solo en [`BeforeCalculate`](./beforecalculate/) y [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Indica si el valor de la celda ha cambiado después del cálculo. Debe usarse solo en [`AfterCalculate`](./aftercalculate/). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implementa este método para realizar acciones después de que se haya calculado una celda. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implementa este método para realizar acciones antes de calcular una celda. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implemente este método para realizar operaciones al calcular fórmulas con referencias circulares. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Implementación personalizada de AbstractCalculationMonitor
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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Crear una instancia de CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Establecer opciones de cálculo
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Calcular fórmulas con el monitor personalizado
            workbook.CalculateFormula(options);

            // Guarda el libro de trabajo
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


