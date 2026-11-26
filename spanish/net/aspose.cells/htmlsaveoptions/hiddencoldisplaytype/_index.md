---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Columna oculta: el ancho de esta columna es 0 en Excel antes de guardarla en formato html. Si HtmlHiddenColDisplayType es Remove, la columna oculta no se exportará; si el valor es Hidden, la columna se exportará pero permanecerá oculta. El valor predeterminado es Hidden."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se exportará; si el valor es "Hidden", la columna se exportará pero permanecerá oculta. El valor predeterminado es "Hidden".

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ocultar la columna C (índice 2)
            worksheet.Cells.HideColumn(2);

            // Agregue algunos datos para demostrar
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // Crear opciones de guardado HTML con diferentes configuraciones de HiddenColDisplayType
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Guardar con diferentes opciones
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### Ver también

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


