---
title: "Style.Pattern"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece el tipo de patrón de fondo de la celda"
type: docs
url: /es/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Obtiene o establece el tipo de patrón de fondo de la celda.

```csharp
public BackgroundType Pattern { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Acceder a la celda y obtener su estilo
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Establecer el patrón y el color de primer plano
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


