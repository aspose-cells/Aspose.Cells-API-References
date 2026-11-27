---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger det informativa namnet på dokumentmallen"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Hämtar eller anger det informativa namnet på dokumentmallen.

```csharp
public string Template { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ange Template-egenskapen
            builtInProperties.Template = "Standard Template";

            // Ställ in andra grundläggande egenskaper för demonstration
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Spara arbetsboken
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


