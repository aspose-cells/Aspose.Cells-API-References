---
title: "WorksheetCollection.ExternalLinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Representa enlaces externos en un libro de trabajo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Representa enlaces externos en un libro de trabajo.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo fuente con enlace externo
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Cree un libro de trabajo de destino
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Establecer la fuente de datos del enlace externo
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Guarda el libro de trabajo
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Limpiar
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### Ver también

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


