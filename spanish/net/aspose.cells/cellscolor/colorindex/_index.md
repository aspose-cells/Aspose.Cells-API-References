---
title: "CellsColor.ColorIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsColor. Obtiene y establece el índice de color en la paleta de colores. Solo se aplica a colores indexados"
type: docs
url: /es/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Obtiene y establece el índice de color en la paleta de colores. Solo se aplica a colores indexados.

```csharp
public int ColorIndex { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definir un rango al que aplicaremos un borde coloreado
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Crear una instancia de CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Establecer el ColorIndex (índice de paleta) – por ejemplo, 5
            cellsColor.ColorIndex = 5;

            // Aplicar CellsColor como el color del borde interno del rango
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Leer y mostrar el valor actual de ColorIndex
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Guardar el libro de trabajo para visualizar el resultado
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


