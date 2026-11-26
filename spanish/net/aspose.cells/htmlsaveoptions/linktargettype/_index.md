---
title: "HtmlSaveOptions.LinkTargetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica el tipo del atributo target en un enlace. El valor predeterminado es HtmlLinkTargetType.Parent"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

Indica el tipo del atributo target en el enlace `<a>`. El valor predeterminado es HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Link to Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");

            // Establecer las opciones de guardado HTML con LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            // Guarda el libro de trabajo como HTML
            workbook.Save("output.html", saveOptions);
        }
    }
}
```

### Ver también

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


