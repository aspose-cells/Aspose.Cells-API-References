---
title: "Clase SolidFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.SolidFill. Encapsula el objeto que representa el formato de relleno sólido"
type: docs
url: /es/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Encapsula el objeto que representa el formato de relleno sólido.

```csharp
public class SolidFill : Fill
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Obtiene y establece el objeto [`CellsColor`](./cellscolor/). |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Obtiene o establece el Color. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Obtiene el código hash. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma rectangular simple a la hoja
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Configurar la forma para usar un relleno sólido
                rect.Fill.FillType = FillType.Solid;

                // Obtener el objeto SolidFill
                SolidFill solidFill = rect.Fill.SolidFill;

                // Establecer propiedades de relleno sólido
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Acceda a la propiedad CellsColor (lectura/escritura)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Guarde el libro de trabajo para verificar la apariencia de la forma
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


