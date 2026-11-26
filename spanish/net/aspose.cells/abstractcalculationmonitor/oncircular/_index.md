---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractCalculationMonitor. Implementa este método para realizar operaciones al calcular fórmulas con referencias circulares"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Implemente este método para realizar operaciones al calcular fórmulas con referencias circulares.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator con elementos [`CalculationCell`](../../calculationcell/) que representan celdas que dependen de referencias circulares. |

### Valor de retorno

Indica si el motor de fórmulas necesita calcular esas celdas en forma circular después de esta llamada. Verdadero para permitir que el motor de fórmulas continúe calculándolas. Falso para que el motor de fórmulas solo marque esas celdas como Calculadas.

### Observaciones

En la implementación, el usuario también puede establecer el valor esperado como resultado calculado para parte/todas esas celdas, de modo que el motor de fórmulas no las calcule recursivamente.

### Ejemplos

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

            // Crear un escenario de referencia circular
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

### Ver también

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


