---
title: "FileFormatInfo.FileFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FileFormatInfo. Obtiene el formato de archivo detectado"
type: docs
url: /es/net/aspose.cells/fileformatinfo/fileformattype/
---
## FileFormatInfo.FileFormatType property

Obtiene el formato de archivo detectado.

```csharp
public FileFormatType FileFormatType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Ejemplo 1: Detectar formato Excel 97-2003
            string excelFile = "sample.xls";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);

            // Ejemplo 2: Detectar formato OOXML
            string xlsxFile = "sample.xlsx";
            info = FileFormatUtil.DetectFileFormat(xlsxFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
        }
    }
}
```

### Ver también

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


