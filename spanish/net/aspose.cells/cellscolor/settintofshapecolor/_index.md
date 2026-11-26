---
title: "CellsColor.SetTintOfShapeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsColor. Establece el tono del color de la forma"
type: docs
url: /es/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Establecer el tono del color de la forma

```csharp
public void SetTintOfShapeColor(double tint)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tinte | Double |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Obtener el color de relleno de la forma
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Establecer el color para que se trate como color de forma
                shapeColor.IsShapeColor = true;
                
                // Establecer el tono del color de la forma (el rango válido es -1.0 a 1.0)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Mostrar el efecto cambiando el color de relleno de la forma
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


