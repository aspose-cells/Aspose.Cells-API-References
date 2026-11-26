---
title: "Hyperlink.ScreenTip"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Hyperlink. Devuelve o establece el texto ScreenTip para el hipervínculo especificado"
type: docs
url: /es/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Devuelve o establece el texto de ScreenTip para el hipervínculo especificado.

```csharp
public string ScreenTip { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // Crear un hipervínculo con ScreenTip
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Guarda el libro de trabajo
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### Ver también

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


