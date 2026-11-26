---
title: "PageSetup.PrintArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el rango a imprimir"
type: docs
url: /es/net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Representa el rango a imprimir.

```csharp
public string PrintArea { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(3);
            
            // Establecer el área de impresión a A1:B3
            worksheet.PageSetup.PrintArea = "A1:B3";
            
            // Guardar solo con el área de impresión
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportPrintAreaOnly = true
            };
            
            workbook.Save("PrintAreaDemo.html", options);
            
            Console.WriteLine("Print area demo created successfully.");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


