---
title: "OdsSaveOptions.GeneratorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsSaveOptions. Получает и задает генератор ods‑файла"
type: docs
url: /ru/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Получает и задаёт генератор ODS‑файла.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyGeneratorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Создайте и настройте параметры сохранения ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Сохраните книгу с указанными параметрами
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### См. также

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


