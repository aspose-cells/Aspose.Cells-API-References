---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exporta el contenido de la hoja oculta. El valor predeterminado es verdadero"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // Establecer opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // Guardar sin exportar la hoja oculta
            workbook.Save("output_without_hidden.html", saveOptions);

            // Cambiar la opción para exportar hojas ocultas
            saveOptions.ExportHiddenWorksheet = true;

            // Guardar con la hoja oculta exportada
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


