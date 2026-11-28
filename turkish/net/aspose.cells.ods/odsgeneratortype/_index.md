---
title: "Enum OdsGeneratorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsGeneratorType enum. ODS oluşturucunun tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

ODS üreticisinin türünü temsil eder.

```csharp
public enum OdsGeneratorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsClassOdsGeneratorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
            
            workbook.Save("OdsGeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


