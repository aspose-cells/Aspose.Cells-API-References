---
title: "Enumeración PageOrientationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.PageOrientationType. Representa constantes de orientación de impresión"
type: docs
url: /es/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Representa las constantes de orientación de impresión.

```csharp
public enum PageOrientationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Landscape | `0` | Orientación horizontal |
| Portrait | `1` | Orientación vertical |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo del libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda al objeto PageSetup de la hoja de cálculo
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establezca la orientación de la página a Horizontal
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Guardar el libro de trabajo en un archivo
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Establezca la orientación de la página a Vertical
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Guarde el libro de trabajo en un archivo diferente
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


