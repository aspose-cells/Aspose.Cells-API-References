---
title: "Enumeración TargetModeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.TargetModeType. Representa el tipo de modo de destino"
type: docs
url: /es/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Representa el tipo de modo de destino.

```csharp
public enum TargetModeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| External | `0` | Enlace externo |
| FilePath | `1` | Rutas locales y completas a archivos o carpetas. |
| Email | `2` | Correo electrónico. |
| CellReference | `3` | Enlace en celda o rango con nombre. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un hipervínculo externo
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Obtener el hipervínculo y comprobar su TargetModeType
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Eliminar el hipervínculo
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


