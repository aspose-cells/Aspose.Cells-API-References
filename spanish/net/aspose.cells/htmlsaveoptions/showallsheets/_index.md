---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se muestran todas las hojas al guardar como un único archivo HTML"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Indica si se muestran todas las hojas al guardar como un único archivo HTML.

```csharp
public bool ShowAllSheets { get; set; }
```

### Observaciones

Solo funciona cuando [`SaveAsSingleFile`](../saveassinglefile/) es True.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con varias hojas
            Workbook workbook = new Workbook();
            
            // Agregar datos a la primera hoja
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // Agregar segunda hoja
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Agregar tercera hoja
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer la propiedad ShowAllSheets en true para exportar todas las hojas
            saveOptions.ShowAllSheets = true;

            // Guardar libro de trabajo con todas las hojas visibles en HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


