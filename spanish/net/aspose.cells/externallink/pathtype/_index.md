---
title: "ExternalLink.PathType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLink. Obtenga el tipo de ruta de este enlace externo"
type: docs
url: /es/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Obtener el tipo de ruta de este enlace externo

```csharp
public string PathType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crear un enlace externo a otro libro de trabajo
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Obtener el enlace externo
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Mostrar el tipo de ruta del enlace externo
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


