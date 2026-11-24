---
title: "Enum OdsGeneratorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsGeneratorType enum. Stellt den Typ des ODS-Generators dar"
type: docs
url: /de/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Stellt den Typ des ODS‑Generators dar.

```csharp
public enum OdsGeneratorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


