---
title: "Style.IsGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si el sombreado de la celda es un patrón de degradado"
type: docs
url: /es/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Indica si el sombreado de la celda es un patrón degradado.

```csharp
public bool IsGradient { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo
            Style style = workbook.CreateStyle();
            
            // Establecer fondo degradado
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Aplicar el estilo a una celda
            worksheet.Cells["A1"].SetStyle(style);
            
            // Verificar si el estilo tiene degradado
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Mostrar el resultado
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Guarda el libro de trabajo
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


