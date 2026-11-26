---
title: "CalculationCell.Cell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationCell. Obtiene el objeto Cell que se está calculando"
type: docs
url: /es/net/aspose.cells/calculationcell/cell/
---
## CalculationCell.Cell property

Obtiene el objeto Cell que está siendo calculado.

```csharp
public Cell Cell { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Crear una instancia de CalculationCell usando reflexión ya que el constructor no es público
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Mostrar el valor de la propiedad Cell
                Console.WriteLine("Cell Name: " + calcCell.Cell.Name);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);
                Console.WriteLine("Cell StringValue: " + calcCell.Cell.StringValue);
                Console.WriteLine("Cell Row: " + calcCell.Cell.Row);
                Console.WriteLine("Cell Column: " + calcCell.Cell.Column);
                Console.WriteLine("Cell IsFormula: " + calcCell.Cell.IsFormula);

                // Demuestre propiedades relacionadas para contexto
                Console.WriteLine("CellRow: " + calcCell.CellRow);
                Console.WriteLine("CellColumn: " + calcCell.CellColumn);

                // Guarda el libro de trabajo
                workbook.Save("CellDemo.xlsx");
                Console.WriteLine("Cell property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


