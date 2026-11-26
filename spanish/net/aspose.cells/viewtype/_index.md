---
title: "Enumeración ViewType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ViewType enum. Representa el tipo de vista de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/viewtype/
---
## ViewType enumeration

Representa el tipo de vista de la hoja de cálculo.

```csharp
public enum ViewType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el tipo de vista de la hoja de cálculo a PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Guarda el libro de trabajo
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


