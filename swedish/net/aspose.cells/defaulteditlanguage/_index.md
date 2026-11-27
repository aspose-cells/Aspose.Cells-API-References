---
title: "Enum DefaultEditLanguage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DefaultEditLanguage enum. Representerar det standardredigeringsspråket"
type: docs
url: /sv/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Representerar standardspråket för redigering.

```csharp
public enum DefaultEditLanguage
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Auto | `0` | Representerar automatisk upptäckt av redigeringsspråk enligt texten själv. |
| English | `1` | Representerar engelska språket. |
| CJK | `2` | Representerar kinesiska, japanska och koreanska språk. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa AutoFitterOptions och ange DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Tillämpa automatisk anpassning av rader med de angivna alternativen
            worksheet.AutoFitRows(autoFitterOptions);

            // Spara arbetsboken
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Skriv ut den angivna DefaultEditLanguage till konsolen
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


