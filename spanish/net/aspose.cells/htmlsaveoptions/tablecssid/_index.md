---
title: "HtmlSaveOptions.TableCssId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene y establece el prefijo del nombre CSS del tipo, como trcoltd, etc., que se encuentran en el elemento table que tiene el atributo TableCssId específico. El valor predeterminado es"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Obtiene y establece el prefijo del nombre CSS del tipo, como tr, col, td, etc., que están contenidos en el elemento table que tiene el atributo TableCssId específico. El valor predeterminado es "".

```csharp
public string TableCssId { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyTableCssIdDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Configurar opciones de guardado HTML con TableCssId
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.TableCssId = "custom-table-style";
            
            // Guardar el libro de trabajo con opciones HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


