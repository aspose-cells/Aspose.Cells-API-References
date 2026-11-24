---
title: "OdsSaveOptions.GeneratorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsSaveOptions‑Eigenschaft. Gibt den Generator der ODS-Datei zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Liest und setzt den Generator der ODS-Datei.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Erstellen und konfigurieren Sie ODS‑Speicheroptionen
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Speichern Sie die Arbeitsmappe mit den angegebenen Optionen
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Siehe auch

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


