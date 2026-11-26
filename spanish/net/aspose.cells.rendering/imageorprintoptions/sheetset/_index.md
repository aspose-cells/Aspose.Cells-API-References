---
title: "ImageOrPrintOptions.SheetSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece las hojas a renderizar. El predeterminado es todas las hojas visibles en el libro de trabajo Visible"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/sheetset/
---
## ImageOrPrintOptions.SheetSet property

Obtiene o establece las hojas a renderizar. El predeterminado es todas las hojas visibles en el libro de trabajo: [`Visible`](../../sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Observaciones

El conjunto se ignora cuando se usa en [`SheetRender`](../../sheetrender/)

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "VisibleSheet1";
            sheet1.Cells["A1"].PutValue("Sheet1 Content");
            
            Worksheet sheet2 = workbook.Worksheets.Add("VisibleSheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Content");
            
            Worksheet sheet3 = workbook.Worksheets.Add("HiddenSheet");
            sheet3.Cells["A1"].PutValue("Hidden Content");
            sheet3.IsVisible = false;

            // Demostrar la propiedad SheetSet con ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;

            // Opción 1: Imprimir todas las hojas (incluyendo ocultas)
            options.SheetSet = SheetSet.All;
            WorkbookRender allSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"All sheets page count: {allSheetsRender.PageCount}");

            // Opción 2: Imprimir solo las hojas visibles
            options.SheetSet = SheetSet.Visible;
            WorkbookRender visibleSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Visible sheets page count: {visibleSheetsRender.PageCount}");

            // Opción 3: Imprimir hojas específicas por índice
            options.SheetSet = new SheetSet(new int[] { 0, 2 }); // First and third sheets
            WorkbookRender specificSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Specific sheets page count: {specificSheetsRender.PageCount}");

            // Guardar una página en el flujo como demostración
            using (MemoryStream stream = new MemoryStream())
            {
                specificSheetsRender.ToImage(0, stream);
                Console.WriteLine($"Image stream length: {stream.Length} bytes");
            }
        }
    }
}
```

### Ver también

* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


