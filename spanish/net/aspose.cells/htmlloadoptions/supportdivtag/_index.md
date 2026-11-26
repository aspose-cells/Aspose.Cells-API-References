---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Indica si se admite el diseño de la etiqueta div cuando el archivo HTML la contiene. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Indica si se admite el diseño de la etiqueta `<div>` cuando el archivo html lo contiene. El valor predeterminado es false.

```csharp
public bool SupportDivTag { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML con SupportDivTag habilitado
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // Cargar archivo HTML con etiquetas div
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // Acceder a los datos de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Salida del valor de celda e información de estilo
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Guardar como archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


