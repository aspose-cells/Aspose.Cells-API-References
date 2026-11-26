---
title: "Class MsoLineFormatHelper"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.MsoLineFormatHelper class. Representa el formato de línea y de punta de flecha"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Representa el formato de línea y punta de flecha.

```csharp
public class MsoLineFormatHelper
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Obtiene y establece el color de fondo de la línea del borde. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Obtiene o establece el estilo de guión para la línea especificada. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Obtiene y establece el color de primer plano de la línea del borde. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Indica si el objeto es visible. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Devuelve un objeto Style que representa el estilo del rango especificado. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 (opaco) a 1.0 (claro). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Devuelve o establece el grosor de la línea, en unidades de pt. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una forma para demostrar el formato de línea
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Obtén el formato de línea directamente de la forma
                MsoLineFormat lineFormat = shape.LineFormat;

                // Establece propiedades directamente en el formato de línea
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Muestra las propiedades configuradas
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Guarda el libro de trabajo
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


