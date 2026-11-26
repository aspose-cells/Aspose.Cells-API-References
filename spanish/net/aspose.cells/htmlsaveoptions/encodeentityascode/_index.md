---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si las entidades de caracteres HTML se reemplazan con código decimal. Por ejemplo, nbsp se reemplaza con 160. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

Indica si las entidades de caracteres html se reemplazan con código decimal. (p.ej., "&amp;nbsp;" se reemplaza con "&amp;#160;"). El valor predeterminado es false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con caracteres especiales
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // Crear opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Mostrar el valor actual de EncodeEntityAsCode
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // Establecer EncodeEntityAsCode en true
            options.EncodeEntityAsCode = true;

            // Guardar con entidades codificadas como código
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // Establecer EncodeEntityAsCode en false
            options.EncodeEntityAsCode = false;

            // Guardar con entidades tal como están
            workbook.Save("HtmlWithRawEntities.html", options);

            // Comparar los archivos de salida
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


