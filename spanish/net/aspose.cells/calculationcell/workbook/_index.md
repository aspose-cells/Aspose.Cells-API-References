---
title: "CalculationCell.Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationCell. Obtiene el objeto Workbook"
type: docs
url: /es/net/aspose.cells/calculationcell/workbook/
---
## CalculationCell.Workbook property

Obtiene el objeto Workbook.

```csharp
public Workbook Workbook { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorkbookDemo
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

                // Mostrar el valor de la propiedad Workbook
                Console.WriteLine("Workbook Name: " + calcCell.Workbook.FileName);
                Console.WriteLine("Workbook Has Macro: " + calcCell.Workbook.HasMacro);
                Console.WriteLine("Workbook Worksheet Count: " + calcCell.Workbook.Worksheets.Count);

                // Demuestre propiedades relacionadas para contexto
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Guarda el libro de trabajo
                workbook.Save("WorkbookDemo.xlsx");
                Console.WriteLine("Workbook property demonstration completed successfully.");
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

* class [Workbook](../../workbook/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


