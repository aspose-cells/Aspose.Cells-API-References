---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger dokumentets språk"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Hämtar eller anger dokumentets språk.

```csharp
public string Language { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till den inbyggda samlingen av dokumentegenskaper
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ställ in språkegenskapen
            builtInProperties.Language = "en-US";

            // Ställ in andra grundläggande egenskaper för demonstration
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Spara arbetsboken
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


