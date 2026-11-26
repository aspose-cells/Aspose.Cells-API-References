---
title: "HtmlSaveOptions.ExportSimilarBorderStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exporta el estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSimilarBorderStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con bordes
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["B1"].PutValue("Similar Border");
            worksheet.Cells["B1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["C1"].PutValue("Different Border");
            worksheet.Cells["C1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Thin));

            // Crear opciones de guardado HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                ExportSimilarBorderStyle = true // Demonstrate the property
            };

            // Guarda el libro de trabajo
            workbook.Save("output.html", htmlSaveOptions);
        }

        private static Style CreateBorderStyle(Workbook workbook, CellBorderType borderType)
        {
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = borderType;
            style.Borders[BorderType.BottomBorder].LineStyle = borderType;
            style.Borders[BorderType.LeftBorder].LineStyle = borderType;
            style.Borders[BorderType.RightBorder].LineStyle = borderType;
            return style;
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


