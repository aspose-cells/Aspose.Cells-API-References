---
title: "HtmlSaveOptions.ExportExtraHeadings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan encabezados extra cuando la longitud del texto es mayor que la columna de visualización máxima. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Indica si se exportan encabezados adicionales cuando la longitud del texto supera la columna de visualización máxima. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y encabezados extra
            worksheet.Cells["A1"].PutValue("Main Heading");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");
            
            // Establecer encabezados extra (filas y columnas)
            worksheet.Cells["Z1"].PutValue("Extra Column Heading");
            worksheet.Cells["A100"].PutValue("Extra Row Heading");

            // Configurar opciones de guardado HTML con ExportExtraHeadings
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportHeadings = true;
            saveOptions.ExportExtraHeadings = true;

            // Guardar en HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML exported with extra headings.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


