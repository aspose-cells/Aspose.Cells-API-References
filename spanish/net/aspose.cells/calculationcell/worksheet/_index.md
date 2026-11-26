---
title: "CalculationCell.Worksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationCell. Obtiene el objeto Worksheet donde está la celda"
type: docs
url: /es/net/aspose.cells/calculationcell/worksheet/
---
## CalculationCell.Worksheet property

Obtiene el objeto Worksheet donde se encuentra la celda.

```csharp
public Worksheet Worksheet { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorksheetDemo
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

                // Muestra el valor de la propiedad Worksheet
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Worksheet Index: " + calcCell.Worksheet.Index);
                Console.WriteLine("Worksheet Type: " + calcCell.Worksheet.Type);

                // Demuestre otras propiedades relacionadas
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Guarda el libro de trabajo
                workbook.Save("WorksheetDemo.xlsx");
                Console.WriteLine("Worksheet property demonstration completed successfully.");
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

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


