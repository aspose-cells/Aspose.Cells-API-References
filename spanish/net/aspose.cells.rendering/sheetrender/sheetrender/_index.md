---
title: "SheetRender.SheetRender"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de SheetRender. la construcción de SheetRender necesita worksheet e ImageOrPrintOptions como parámetros"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

la construcción de SheetRender, necesita la hoja de cálculo y ImageOrPrintOptions como parámetros

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| worksheet | Hoja de cálculo | Indique cuál hoja de cálculo se debe renderizar. |
| opciones | ImageOrPrintOptions | ImageOrPrintOptions contiene algunas propiedades de la imagen de salida |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo y agregue algunos datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Cree SheetRender con Worksheet e ImageOrPrintOptions
            SheetRender render = new SheetRender(worksheet, options);

            // Salida del recuento de páginas
            Console.WriteLine("Page count: " + render.PageCount);

            // Guarde la imagen renderizada
            render.ToImage(0, "output.png");
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


