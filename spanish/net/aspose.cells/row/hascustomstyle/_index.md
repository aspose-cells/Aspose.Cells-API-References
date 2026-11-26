---
title: "Row.HasCustomStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Indica si esta fila tiene configuraciones de estilo personalizadas diferentes del estilo predeterminado heredado del libro de trabajo"
type: docs
url: /es/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Indica si esta fila tiene configuraciones de estilo personalizadas(diferentes de la predeterminada heredada del libro de trabajo).

```csharp
public bool HasCustomStyle { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear y personalizar un estilo
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // Acceder a la primera fila
            Row row = worksheet.Cells.Rows[0];
            
            // Aplicar estilo personalizado a la fila
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Verificar si la fila tiene estilo personalizado (debe ser verdadero)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Guarda el libro de trabajo
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


