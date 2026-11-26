---
title: "MarkdownSaveOptions.SheetSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo Active"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Observaciones

El conjunto se ignora cuando se usa en [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("Sheet1 Data");
            
            // Agregar una segunda hoja de cálculo
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Data");

            // Crear opciones de guardado Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Guardar todas las hojas en markdown
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save("output_all_sheets.md", saveOptions);
            
            // Guardar solo la primera hoja
            saveOptions.SheetSet = new SheetSet(new int[] { 0 });
            workbook.Save("output_first_sheet.md", saveOptions);
        }
    }
}
```

### Ver también

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


