---
title: "Style.VerticalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece el tipo de alineación vertical del texto en una celda"
type: docs
url: /es/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Obtiene o establece el tipo de alineación vertical del texto en una celda.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la celda A1
            Cell cell = worksheet.Cells["A1"];
            
            // Establecer el valor de la celda
            cell.PutValue("Vertical Alignment Demo");
            
            // Accede al estilo de la celda
            Style style = cell.GetStyle();
            
            // Establece la alineación vertical a Superior
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


