---
title: "OdsSaveOptions.GeneratorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsSaveOptions. Ottiene e imposta il generatore del file ods"
type: docs
url: /it/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Ottiene e imposta il generatore del file ods.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea e configura le opzioni di salvataggio ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Salva la cartella di lavoro con le opzioni specificate
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Vedi anche

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


