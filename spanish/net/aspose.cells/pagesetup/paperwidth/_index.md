---
title: "PageSetup.PaperWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Obtiene el ancho del papel en unidades de pulgadas según la orientación de la página"
type: docs
url: /es/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Obtiene el ancho del papel en unidades de pulgadas, considerada la orientación de la página.

```csharp
public double PaperWidth { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Acceder al PageSetup de la hoja de cálculo
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Demostrar la propiedad PaperWidth (solo lectura)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // Para cambiar el tamaño del papel, use la propiedad PaperSize en su lugar
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


