---
title: "SheetRender.PageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SheetRender. Obtiene el recuento total de páginas de la hoja de cálculo actual"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Obtiene el recuento total de páginas de la hoja de cálculo actual.

```csharp
public int PageCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Establecer la configuración de página para imprimir
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // Crear SheetRender con opciones predeterminadas
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Mostrar el recuento de páginas
            Console.WriteLine("Page Count: " + render.PageCount);

            // Cambiar la configuración de página para forzar varias páginas
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Crear un nuevo SheetRender para obtener el recuento de páginas actualizado
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


