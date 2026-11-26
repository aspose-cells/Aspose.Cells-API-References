---
title: "OoxmlSaveOptions.CompressionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OoxmlSaveOptions. Получает и задаёт тип сжатия для файла ooxml"
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/compressiontype/
---
## OoxmlSaveOptions.CompressionType property

Получает и задает тип сжатия для файла ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Примечания

Значение по умолчанию — OoxmlCompressionType.Level2.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyCompressionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Compression Test");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;

            workbook.Save("CompressionDemo.xlsx", saveOptions);
            Console.WriteLine("Workbook saved with Level6 compression.");
        }
    }
}
```

### См. также

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


