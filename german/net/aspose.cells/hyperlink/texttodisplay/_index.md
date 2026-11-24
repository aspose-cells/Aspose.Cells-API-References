---
title: "Hyperlink.TextToDisplay"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Hyperlink-Eigenschaft. Stellt den anzuzeigenden Text für den angegebenen Hyperlink dar. Der Standardwert ist die Adresse des Hyperlinks"
type: docs
url: /de/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Stellt den Text dar, der für den angegebenen Hyperlink angezeigt wird. Der Standardwert ist die Adresse des Hyperlinks.

```csharp
public string TextToDisplay { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hyperlinks mit der TextToDisplay-Eigenschaft hinzufügen
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Ersten Hyperlink mit benutzerdefiniertem Anzeigetext hinzufügen
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Zweiten Hyperlink mit benutzerdefiniertem Anzeigetext hinzufügen
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Dritten Hyperlink mit Zellreferenz als Anzeigetext hinzufügen
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Speichere die Arbeitsmappe
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


