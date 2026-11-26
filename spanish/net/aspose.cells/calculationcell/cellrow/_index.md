---
title: "CalculationCell.CellRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationCell. Obtiene el índice de fila de la celda"
type: docs
url: /es/net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Obtiene el índice de fila de la celda.

```csharp
public int CellRow { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellRowDemo
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

                // Muestra el valor de la propiedad CellRow
                Console.WriteLine("CellRow value: " + calcCell.CellRow);

                // Demuestre propiedades relacionadas para contexto
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);

                // Guarda el libro de trabajo
                workbook.Save("CellRowDemo.xlsx");
                Console.WriteLine("CellRow property demonstration completed successfully.");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


