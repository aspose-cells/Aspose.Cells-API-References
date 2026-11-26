---
title: "Перечисление OdsGeneratorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Ods.OdsGeneratorType. Представляет тип генератора ODS"
type: docs
url: /ru/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Представляет тип генератора ODS.

```csharp
public enum OdsGeneratorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Примеры

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

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


