---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Indica se supportare il layout del tag div quando il file HTML lo contiene. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Indica se supportare il layout del tag `<div>` quando il file HTML lo contiene. Il valore predefinito è false.

```csharp
public bool SupportDivTag { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento HTML con SupportDivTag abilitato
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // Carica il file HTML con tag div
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // Accedi ai dati dal primo worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Restituisci il valore della cella e le informazioni di stile
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Salva come file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


