---
title: "CalculationCell.CellColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationCell. Obtiene el índice de columna de la celda"
type: docs
url: /es/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Obtiene el índice de columna de la celda.

```csharp
public int CellColumn { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Introducir algunos datos y una fórmula simple
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Obtener una instancia de CalculationCell mediante reflexión (su constructor no es público)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Leer y mostrar el valor de la propiedad CellColumn
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Demostración adicional de propiedades relacionadas (opcional)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Guardar el libro de trabajo (el archivo contendrá los datos que añadimos)
                workbook.Save("CellColumnDemo.xlsx");
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


