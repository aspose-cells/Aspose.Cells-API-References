---
title: "Style.ForegroundArgbColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene y establece el color de primer plano con un valor ARGB de 32 bits"
type: docs
url: /es/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Obtiene y establece el color de primer plano con un valor ARGB de 32 bits.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un estilo con un color de primer plano específico
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Obtener y mostrar el valor del color ARGB de primer plano
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Guarda el libro de trabajo
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


