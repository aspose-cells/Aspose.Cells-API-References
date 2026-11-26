---
title: "PaginatedSaveOptions.SheetSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo Visible"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Establezca algunos datos de muestra en ambas hojas
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Guarde solo la segunda hoja usando SheetSet
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // Guarda el libro de trabajo con las hojas especificadas
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


