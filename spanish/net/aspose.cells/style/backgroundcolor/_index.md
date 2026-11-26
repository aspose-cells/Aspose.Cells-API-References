---
title: "Style.BackgroundColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece el color de fondo de un estilo"
type: docs
url: /es/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Obtiene o establece el color de fondo de un estilo.

```csharp
public Color BackgroundColor { get; set; }
```

### Observaciones

Si deseas establecer el color de una celda, por favor usa la propiedad Style.ForegroundColor. Solo si el patrón de estilo de la celda es distinto de ninguno o sólido, esta propiedad tendrá efecto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cree un objeto de estilo
            Style style = workbook.CreateStyle();
            
            // Establece el color de fondo a amarillo
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Aplicar el estilo a la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


