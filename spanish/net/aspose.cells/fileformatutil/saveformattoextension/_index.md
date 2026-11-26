---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Convierte un valor enumerado de formato de guardado en una extensión de archivo"
type: docs
url: /es/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Convierte un valor enumerado de formato de guardado en una extensión de archivo.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formato | SaveFormat | El formato de guardado. |

### Valor de retorno

La extensión devuelta es una cadena en minúsculas con un punto inicial.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // Demostrar SaveFormatToExtension con diferentes formatos
            SaveOptions[] saveOptions = {
                new PdfSaveOptions(),
                new XlsSaveOptions(SaveFormat.Excel97To2003),
                new OoxmlSaveOptions(SaveFormat.Xlsx),
                new OdsSaveOptions()
            };

            foreach (var options in saveOptions)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
                Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
                
                // Guardar con la extensión detectada
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


