---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Hämtar eller anger standardspråk för redigering"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Hämtar eller anger standardspråket för redigering.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Anmärkningar

Den kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är Auto.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempel på CJK-text i en cell
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Autoanpassa rad med CJK-språkinställningar
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


