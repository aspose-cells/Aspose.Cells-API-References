---
title: "Enumeración HtmlVersion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.HtmlVersion. Indica la versión de HTML que se usa al guardar en formatos HTML"
type: docs
url: /es/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

Indica la versión de HTML que se usa al guardar en formatos HTML.

```csharp
public enum HtmlVersion
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Guarde el documento cumpliendo con la exportación HTML de MS Excel. |
| XHtml | `1` | Guarda el documento cumpliendo con el estándar XHTML 1.0 Transitional. |
| Html5 | `2` | Guarda el documento cumpliendo con el estándar HTML 5. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Establecer la versión HTML a HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Guardar el libro con la versión HTML5
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // Cambiar la versión HTML a XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Guardar el libro con la versión XHTML
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // Establecer la versión HTML a Predeterminada (compatible con MS Excel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Guardar el libro con la versión Predeterminada
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


