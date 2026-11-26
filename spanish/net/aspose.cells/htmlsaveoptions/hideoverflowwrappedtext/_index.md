---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se oculta el texto que se desborda cuando el formato de la celda está configurado para envolver texto. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Indica si se debe ocultar el texto que se desborda cuando el formato de la celda está configurado para ajustar texto. El valor predeterminado es false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer texto de ejemplo en la celda A1
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Crear y aplicar estilo con ajuste de texto
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Obtener la colección de celdas y aplicar estilo
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Establecer el ancho de columna para que el texto se ajuste
            cells.SetColumnWidth(0, 10);
            
            // Crear opciones de guardado HTML y establecer HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Guardar libro con opciones HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


