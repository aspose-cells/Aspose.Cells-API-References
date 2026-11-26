---
title: "Clase ExternalLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExternalLink. Representa un enlace externo en un libro de trabajo"
type: docs
url: /es/net/aspose.cells/externallink/
---
## ExternalLink class

Representa un enlace externo en un libro de trabajo.

```csharp
public class ExternalLink
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Representa la fuente de datos del enlace externo. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Indica si este enlace externo es referenciado por otros. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Indica si este enlace externo es visible en MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Representa la fuente de datos almacenada del enlace externo. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Obtener el tipo de ruta de este enlace externo |
| [Type](../../aspose.cells/externallink/type/) { get; } | Obtiene el tipo de enlace externo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Agrega un nombre externo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Abrir un archivo con enlaces externos
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Obtener enlace externo 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Mostrar propiedades del enlace externo
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Cambiar la fuente de datos del enlace externo
            externalLink.DataSource = "d:\\linktest.xls";

            // Agregar un nombre externo al enlace externo
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Guarda el libro de trabajo
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


