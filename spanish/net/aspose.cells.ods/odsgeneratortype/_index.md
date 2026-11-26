---
title: "Enumeración OdsGeneratorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Ods.OdsGeneratorType. Representa el tipo de generador ODS"
type: docs
url: /es/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Representa el tipo de generador de ODS.

```csharp
public enum OdsGeneratorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


