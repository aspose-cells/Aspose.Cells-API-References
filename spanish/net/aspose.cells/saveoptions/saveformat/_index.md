---
title: "SaveOptions.SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Obtiene el formato de archivo guardado"
type: docs
url: /es/net/aspose.cells/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Obtiene el formato de archivo de guardado.

```csharp
public SaveFormat SaveFormat { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Demostrar diferentes formatos de guardado
            SaveOptions[] options = {
                new PdfSaveOptions(),
                new OoxmlSaveOptions(),
                new HtmlSaveOptions()
            };

            foreach (var saveOptions in options)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
                Console.WriteLine($"Saving as {saveOptions.SaveFormat} with extension: {extension}");

                string outputPath = $"output_{Guid.NewGuid().ToString("N").Substring(0, 8)}{extension}";
                workbook.Save(outputPath, saveOptions);
                Console.WriteLine($"Saved to: {outputPath}");
            }

            // Limpiar
            workbook.Dispose();
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


