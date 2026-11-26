---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si una cadena cruzada de celda se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato html. Por defecto el valor es Default, por lo que para cadenas cruzadas de celda hay poca diferencia entre los archivos html creados por Aspose.Cells y MS Excel. Pero el rendimiento al crear archivos html grandes estableciendo el valor a Cross sería varias veces más rápido que establecerlo a Default o Fit2Cell"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Indica si una cadena que abarca varias celdas se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato HTML. Por defecto el valor es Default, por lo que, para cadenas que cruzan celdas, hay poca diferencia entre los archivos HTML creados por Aspose.Cells y MS Excel. Sin embargo, el rendimiento al crear archivos HTML grandes, al establecer el valor en Cross sería varias veces más rápido que establecerlo en Default o Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo que demuestren el comportamiento de cadenas cruzadas
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Obtener y modificar estilos de celda
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // Configurar opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Guardar el libro de trabajo en HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### Ver también

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


