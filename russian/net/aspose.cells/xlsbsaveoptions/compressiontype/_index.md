---
title: "XlsbSaveOptions.CompressionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XlsbSaveOptions. Получает и задаёт тип сжатия для файла ooxml"
type: docs
url: /ru/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Получает и задает тип сжатия для файла ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Примечания

Значение по умолчанию — OoxmlCompressionType.Level6.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyCompressionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Compression Test");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6
            };

            workbook.Save("XlsbWithCompression.xlsb", saveOptions);
        }
    }
}
```

### См. также

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


