---
title: "CalculationData.CellRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationData. Obtiene el índice de fila de la celda donde está la función"
type: docs
url: /es/net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

Obtiene el índice de fila de la celda donde está la función.

```csharp
public int CellRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos de muestra
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Establecer opciones de cálculo
            CalculationOptions opts = new CalculationOptions();
            opts.CustomEngine = new CustomCalculationEngine();

            // Calcular fórmulas
            workbook.CalculateFormula(opts);

            // Acceder a la celda calculada y demostrar la propiedad CellRow
            Cell calculatedCell = worksheet.Cells["A3"];
            Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Demostrar el acceso a la información de fila desde los datos de cálculo
            if (data != null)
            {
                Console.WriteLine("Current calculation is for row: " + data.CellRow);
            }
        }
    }
}
```

### Ver también

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


