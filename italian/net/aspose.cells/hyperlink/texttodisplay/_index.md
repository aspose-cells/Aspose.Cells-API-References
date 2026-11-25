---
title: "Hyperlink.TextToDisplay"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Hyperlink. Rappresenta il testo da visualizzare per l'hyperlink specificato. Il valore predefinito è l'indirizzo dell'hyperlink"
type: docs
url: /it/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. Il valore predefinito è l'indirizzo del collegamento ipertestuale.

```csharp
public string TextToDisplay { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi hyperlink con la proprietà TextToDisplay
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Aggiungi il primo hyperlink con testo di visualizzazione personalizzato
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Aggiungi il secondo collegamento ipertestuale con testo di visualizzazione personalizzato
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Aggiungi il terzo collegamento ipertestuale con riferimento di cella come testo di visualizzazione
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Salva la cartella di lavoro
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


