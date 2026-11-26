---
title: "PageSetup.PaperHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Obtiene la altura del papel en unidades de pulgadas, considerando la orientación de la página"
type: docs
url: /es/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Obtiene la altura del papel en unidades de pulgadas, considerada la orientación de la página.

```csharp
public double PaperHeight { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunos datos en una celda
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // Obtener el objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Mostrar la altura de papel predeterminada (en pulgadas)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight es de solo lectura, por lo que demostramos cómo obtener diferentes tamaños de papel
            // cambiando el tipo de tamaño de papel a Letter (8.5x11 pulgadas)
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Verificar el cambio
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


