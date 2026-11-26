---
title: "HtmlSaveOptions.PresentationPreference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true.

```csharp
public bool PresentationPreference { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Presentation Preference Test");
            worksheet.Cells["B1"].PutValue(123.45);
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // Establecer opciones de guardado HTML con PresentationPreference
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = false;

            // Guardar en un flujo de memoria para demostración
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                Console.WriteLine("Workbook saved with PresentationPreference=true");
            }
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


