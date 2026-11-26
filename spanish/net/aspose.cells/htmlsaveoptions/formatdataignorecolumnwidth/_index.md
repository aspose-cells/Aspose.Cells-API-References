---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. Si es true, se ignora el ancho de columna y se exportará todo el dato de la celda. Si es false, los datos se exportarán igual que en Excel. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. Si es true, se ignora el ancho de columna y se exportará todo el dato de la celda. Si es false, el dato se exportará igual que en Excel. El valor predeterminado es false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de ejemplo y ancho de columna
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Demostrar la propiedad FormatDataIgnoreColumnWidth
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Guardar con diferentes configuraciones para mostrar el efecto
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


