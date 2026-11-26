---
title: "StyleFlag.StyleFlag"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "StyleFlag constructor. Construye un objeto con todas las banderas en false"
type: docs
url: /es/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Construye un objeto con todas las banderas en falso.

```csharp
public StyleFlag()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo en negrita
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Aplicar estilo a la fila 9 con StyleFlag constructor
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Colocar valor en la celda y verificar el estilo
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


