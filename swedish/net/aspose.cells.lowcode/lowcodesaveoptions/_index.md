---
title: "Klass LowCodeSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeSaveOptions class. Alternativ för att spara genererade resultat på lågkodssätt"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Alternativ för att spara genererade resultat på ett lågt kodsätt.

```csharp
public class LowCodeSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Hämtar och anger filen (med sökväg om behövs) för att spara den genererade datan. När den här egenskapen sätts till ett värde annat än null eller tom sträng, kommer [`OutputStream`](./outputstream/) att ignoreras. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Hämtar och anger strömmen för att skriva den genererade datan till. När den här egenskapen sätts till ett värde annat än null, kommer [`OutputFile`](./outputfile/) att ignoreras. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Hämtar och anger sparaformatet för utdata. Generellt, för specifika processer på lågkodssätt, är endast vissa specifika format tillåtna. Ange det korrekta formatet för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och lägg in lite data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Skapa sparalternativ
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Spara arbetsboken med de angivna alternativen
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


