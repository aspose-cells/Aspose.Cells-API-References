---
title: "Enumerazione OdsGeneratorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OdsGeneratorType enum. Rappresenta il tipo di generatore ODS"
type: docs
url: /it/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Rappresenta il tipo di generatore ODS.

```csharp
public enum OdsGeneratorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


