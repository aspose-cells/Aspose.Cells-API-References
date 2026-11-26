---
title: "MsoLineFormat.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormat. Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de arco
            ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);

            // Establecer propiedades de formato de línea incluyendo transparencia
            arc.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc.LineFormat.Transparency = 0.5; // 50% transparent
            arc.LineFormat.Weight = 3;
            arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Crear otro arco para comparación
            ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
            arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc2.LineFormat.Transparency = 0.5; // Same transparency
            arc2.LineFormat.Weight = 3;
            arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Verificar la propiedad de transparencia
            if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
            {
                Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
            }
            else
            {
                Console.WriteLine("Transparency properties do not match");
            }

            // Guarda el libro de trabajo
            workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


