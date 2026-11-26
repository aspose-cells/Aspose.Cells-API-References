---
title: "CalculationData.Cell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationData. Obtiene el objeto Cell donde se encuentra la función"
type: docs
url: /es/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Obtiene el objeto Cell donde está la función.

```csharp
public Cell Cell { get; }
```

### Observaciones

Al calcular una fórmula sin asignarla a una celda, como mediante [`CalculateFormula`](../../worksheet/calculateformula/), la fórmula se calculará como si se hubiera establecido en la celda A1, por lo que tanto [`CellRow`](../cellrow/) como [`CellColumn`](../cellcolumn/) son 0. Sin embargo, la celda A1 en la hoja de cálculo puede no haber sido instanciada. Por lo tanto, en este tipo de situación esta propiedad será nula.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar algunos datos para que el ejemplo tenga sentido
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Crear opciones de cálculo con motor personalizado
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // Calcular fórmulas con opciones
                workbook.CalculateFormula(options);

                // Mostrar el resultado
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Guardar el resultado
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Acceder a la propiedad Cell de solo lectura
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

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
```

### Ver también

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


