---
title: "DocumentProperty.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty‑egenskap. Hämtar eller sätter värdet på egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Hämtar eller anger värdet för egenskapen.

```csharp
public object Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till inbyggda dokumentegenskaper
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Visa de angivna värdena
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


