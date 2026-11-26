---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece el IFilePathProvider para exportar la hoja de cálculo a html por separado."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Obtiene o establece el IFilePathProvider para exportar la hoja de cálculo a html por separado.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y agregar algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crear HtmlSaveOptions y establecer el FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Lógica personalizada para generar rutas de archivo
            return $"custom_{sheetName}";
        }
    }
}
```

### Ver también

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


