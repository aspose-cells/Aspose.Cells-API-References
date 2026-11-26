---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exporta la coordenada de Excel de las celdas no vacías al guardar el archivo en html. El valor predeterminado es false. Si desea importar el html de salida a Excel, mantenga el valor predeterminado."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. El valor predeterminado es false. Si desea importar el html generado a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crear opciones de guardado HTML y habilitar ExportCellCoordinate
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Guardar el libro de trabajo como HTML con coordenadas de celdas
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


