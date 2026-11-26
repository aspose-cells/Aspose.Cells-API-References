---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan las propiedades de la hoja de cálculo.El valor predeterminado es true.Si deseas importar el archivo html o mht a excel, por favor mantén el valor predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Establecer opciones de guardado HTML con ExportWorksheetProperties deshabilitado
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Guardar con propiedades de hoja de cálculo deshabilitadas
            workbook.Save("output_without_worksheet_props.html", options);

            // Habilitar exportación de propiedades de hoja de cálculo
            options.ExportWorksheetProperties = true;
            
            // Guardar con propiedades de hoja de cálculo habilitadas
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


