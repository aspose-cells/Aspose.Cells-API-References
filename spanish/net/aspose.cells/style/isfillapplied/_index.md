---
title: "Style.IsFillApplied"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si se debe aplicar el formato de relleno"
type: docs
url: /es/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Indica si se debe aplicar el formato de relleno.

```csharp
public bool IsFillApplied { get; set; }
```

### Observaciones

Solo para estilo con nombre.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un estilo
            Style style = workbook.CreateStyle();
            
            // Inicialmente, IsFillApplied debe ser false
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Aplicar configuraciones de relleno
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Después de establecer las propiedades de relleno, IsFillApplied debe ser true
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Aplicar el estilo a una celda
            worksheet.Cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


