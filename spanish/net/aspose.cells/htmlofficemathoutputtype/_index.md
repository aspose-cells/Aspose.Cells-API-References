---
title: "Enumeración HtmlOfficeMathOutputType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.HtmlOfficeMathOutputType. Representa cómo exportar OfficeMath a HTML"
type: docs
url: /es/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

Representa cómo exportar OfficeMath a HTML.

```csharp
public enum HtmlOfficeMathOutputType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Image | `0` | Convierte OfficeMath a HTML como imagen especificada por la etiqueta &lt;img&gt;. |
| MathML | `1` | Convierte OfficeMath a HTML usando MathML. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar OfficeMath a la celda A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer el tipo de salida de OfficeMath a Imagen
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Guardar con tipo de salida Imagen
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Cambiar el tipo de salida a MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // Guardar con tipo de salida MathML
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


