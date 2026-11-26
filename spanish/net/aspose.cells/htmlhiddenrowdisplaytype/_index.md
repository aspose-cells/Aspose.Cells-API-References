---
title: "Enum HtmlHiddenRowDisplayType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.HtmlHiddenRowDisplayType. Representa dos tipos de visualización de filas ocultas en HTML"
type: docs
url: /es/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

Representa dos tipos de visualización de filas ocultas en HTML.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Hidden | `0` | Oculta las filas ocultas en la página HTML. |
| Remove | `1` | Elimina las filas ocultas en la página HTML. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // Ocultar la segunda fila
            worksheet.Cells.HideRow(1);

            // Crear HtmlSaveOptions y establecer HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


