---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger hyperlinkbase-egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Hämtar eller anger hyperlinkbase-egenskapen.

```csharp
public string HyperlinkBase { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in HyperlinkBase-egenskapen
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Ställ in någon annan egenskap för demonstration
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Spara arbetsboken
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Skriv ut egenskaperna till konsolen
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


