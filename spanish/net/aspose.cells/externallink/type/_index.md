---
title: "ExternalLink.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLink. Obtiene el tipo de enlace externo"
type: docs
url: /es/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Obtiene el tipo de enlace externo.

```csharp
public ExternalLinkType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crear un enlace externo a otro libro de trabajo
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Obtener el enlace externo
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Mostrar el tipo de enlace externo
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Cambiar la fuente de datos del enlace externo
            externalLink.DataSource = "d:\\link.xls";
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### Ver también

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


