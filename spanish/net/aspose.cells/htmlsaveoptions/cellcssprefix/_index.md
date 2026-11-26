---
title: "HtmlSaveOptions.CellCssPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene y establece el prefijo del nombre CSS. El valor predeterminado es"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

Obtiene y establece el prefijo del nombre css, el valor predeterminado es "".

```csharp
public string CellCssPrefix { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellCssPrefixDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Establecer opciones de guardado HTML con CellCssPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellCssPrefix = "custom-cell-";

            // Guardar el libro de trabajo con opciones HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("HTML file saved with custom cell CSS prefix.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


