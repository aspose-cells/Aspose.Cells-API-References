---
title: "PageSetup.FitToPagesWide"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el número de páginas de ancho al que se escalará la hoja de cálculo cuando se imprima. El valor predeterminado es 1"
type: docs
url: /es/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Representa el número de páginas de ancho a las que se escalará la hoja de cálculo cuando se imprima. El valor predeterminado es 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Observaciones

Debe establecer FitToPagesTall en cero si desea ajustar todas las columnas en una sola página.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Establecer propiedades de configuración de página
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Guarda el libro de trabajo
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


