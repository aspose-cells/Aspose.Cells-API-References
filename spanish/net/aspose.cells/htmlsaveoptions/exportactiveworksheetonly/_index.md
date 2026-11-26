---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si solo se exporta la hoja de cálculo activa a un archivo html. Si es verdadero, solo la hoja activa se exportará al archivo html. Si es falso, todo el libro de trabajo se exportará al archivo html. El valor predeterminado es falso"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Indica si solo se exporta la hoja de cálculo activa a un archivo html. Si es true, solo la hoja activa se exportará a html; si es false, todo el libro de trabajo se exportará a html. El valor predeterminado es false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Agregar datos de ejemplo a ambas hojas
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Establecer opciones de guardado HTML para exportar solo la hoja de cálculo activa
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Establecer la primera hoja de cálculo como activa
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Guardar solo con la hoja de cálculo activa
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Cambiar la hoja activa y guardar nuevamente
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


