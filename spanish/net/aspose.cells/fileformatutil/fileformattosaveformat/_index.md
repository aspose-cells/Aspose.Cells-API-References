---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Convirtiendo el formato de archivo al formato de guardado"
type: docs
url: /es/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Convirtiendo el formato de archivo a formato de guardado.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formato | FileFormatType | El tipo de formato de archivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Obtenga el tipo de formato de archivo del libro de trabajo
            FileFormatType originalFormat = workbook.FileFormat;

            // Convertir FileFormatType a SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Guarde el libro de trabajo usando el SaveFormat convertido
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


