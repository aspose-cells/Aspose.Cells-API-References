---
title: "Hyperlink.TextToDisplay"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hyperlink‑egenskap. Representerar den text som ska visas för den angivna hyperlänken. Standardvärdet är hyperlänkens adress"
type: docs
url: /sv/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Representerar texten som ska visas för den angivna hyperlänken. Standardvärdet är hyperlänkens adress.

```csharp
public string TextToDisplay { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyTextToDisplayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till hyperlänkar med TextToDisplay‑egenskapen
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Lägg till den första hyperlänken med anpassad visningstext
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Lägg till den andra hyperlänken med anpassad visningstext
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Lägg till den tredje hyperlänken med cellreferens som visningstext
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Spara arbetsboken
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### Se även

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


