---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Fila oculta: la altura de esta fila es 0 en Excel antes de guardarla en formato HTML; si HtmlHiddenRowDisplayType es Remove, la fila oculta no se exportará; si el valor es Hidden, la fila se exportará pero permanecerá oculta; el valor predeterminado es Hidden"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato HTML, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se generará, si el valor es "Hidden", la fila se generará pero permanecerá oculta, el valor predeterminado es "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y ocultar una fila
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // Establecer opciones de guardado HTML con HiddenRowDisplayType
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // Guardar en HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### Ver también

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


