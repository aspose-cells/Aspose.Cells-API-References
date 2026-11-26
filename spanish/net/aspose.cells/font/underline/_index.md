---
title: "Font.Underline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece el tipo de subrayado de la fuente"
type: docs
url: /es/net/aspose.cells/font/underline/
---
## Font.Underline property

Obtiene o establece el tipo de subrayado de la fuente.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Acceder a la celda y establecer el estilo de subrayado
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Obtener el estilo y modificar las propiedades de la fuente
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


