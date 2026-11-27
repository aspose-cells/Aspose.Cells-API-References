---
title: "Enum OdsGeneratorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsGeneratorType-enum. Representerar typen av ODS-generator"
type: docs
url: /sv/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Representerar typen av ODS‑generator.

```csharp
public enum OdsGeneratorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


