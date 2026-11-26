---
title: "CalculationData.CellColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationData. Obtiene el índice de columna de la celda donde está la función"
type: docs
url: /es/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Obtiene el índice de columna de la celda donde está la función.

```csharp
public int CellColumn { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de ejemplo con fórmulas en diferentes columnas
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // Crear opciones de cálculo con motor personalizado
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // Calcular fórmulas
                workbook.CalculateFormula(options);

                // Mostrar el resultado calculado
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // Guardar el resultado
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // Acceder a la propiedad de solo lectura CellColumn
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // Demostrar el uso de la información de la columna
                if (data.FunctionName == "SUM")
                {
                    double sum = 0;
                    for (int i = 0; i < data.ParamCount; i++)
                    {
                        object arg = data.GetParamValue(i);
                        if (arg is double)
                        {
                            sum += (double)arg;
                        }
                    }
                    data.CalculatedValue = sum;
                }
            }
        }
    }
}
```

### Ver también

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


