---
title: "Enum HtmlLinkTargetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.HtmlLinkTargetType. Representa el tipo del atributo target en la etiqueta HTML"
type: docs
url: /es/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

Representa el tipo del atributo target en la etiqueta HTML.

```csharp
public enum HtmlLinkTargetType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Blank | `0` | Abre el documento vinculado en una nueva ventana o pestaña |
| Parent | `1` | Abre el documento vinculado en el marco principal |
| Self | `2` | Abre el documento vinculado en el mismo marco en que se hizo clic (este es el valor predeterminado) |
| Top | `3` | Abre el documento vinculado en el cuerpo completo de la ventana |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Crear HtmlSaveOptions y establecer el LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


