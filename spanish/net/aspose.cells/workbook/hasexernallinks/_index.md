---
title: "Workbook.HasExernalLinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Indica si este libro de trabajo contiene enlaces externos a otras fuentes de datos"
type: docs
url: /es/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Indica si este libro de trabajo contiene enlaces externos a otras fuentes de datos.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Valor de retorno

Si este libro de trabajo contiene enlaces externos a otras fuentes de datos.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice ExternalLinkCollection.Count para comprobar si hay enlaces externos en este libro de trabajo. Este método será eliminado 12 meses después de diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con enlaces externos
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Agregar un enlace externo
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Comprobar si el libro de trabajo tiene enlaces externos
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


