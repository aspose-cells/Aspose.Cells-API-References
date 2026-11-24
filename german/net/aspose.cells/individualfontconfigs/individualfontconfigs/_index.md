---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Konstruktor. Ctor"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Ctor.

```csharp
public IndividualFontConfigs()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // Ladeoptionen mit IndividualFontConfigs erstellen
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Erstellen Sie eine neue Arbeitsmappe mit einem Standard-Arbeitsblatt
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Greifen Sie auf ein Arbeitsblatt zu und fügen Sie etwas Text hinzu
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Speichern Sie die Arbeitsmappe (Ladeoptionen sind zum Speichern nicht erforderlich)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### Siehe auch

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


