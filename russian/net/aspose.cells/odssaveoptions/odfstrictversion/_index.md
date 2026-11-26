---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsSaveOptions. Получает и задает версию ODF"
type: docs
url: /ru/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Получает и задаёт версию ODF.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // Создайте параметры сохранения ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // Установите версию ODF 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Сохранить с указанной версией ODF
            workbook.Save("OdfVersion12.ods", saveOptions);

            // Перейдите на версию ODF 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### См. также

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


