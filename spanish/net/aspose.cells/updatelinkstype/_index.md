---
title: "Enum UpdateLinksType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.UpdateLinksType. Representa cómo actualizar los enlaces a otros libros de trabajo cuando se abre el libro de trabajo"
type: docs
url: /es/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Representa cómo actualizar los enlaces a otros libros cuando se abre el libro.

```csharp
public enum UpdateLinksType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| UserSet | `0` | Solicitar al usuario que actualice. |
| Never | `1` | No actualizar y no solicitar al usuario. |
| Always | `2` | Actualizar siempre. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer UpdateLinksType a Actualizar siempre
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Guarda el libro de trabajo
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Mostrar la configuración actual de UpdateLinksType
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


