---
title: "BuiltInDocumentPropertyCollection.Company"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger företagsegenskapen"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/company/
---
## BuiltInDocumentPropertyCollection.Company property

Hämtar eller anger företagsegenskapen.

```csharp
public string Company { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCompanyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in inbyggda dokumentegenskaper inklusive Company
            workbook.BuiltInDocumentProperties.Title = "Annual Report";
            workbook.BuiltInDocumentProperties.Company = "Contoso Ltd";
            
            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx");
            
            // Visa de inställda egenskaperna
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties.Title);
            Console.WriteLine("Company: " + workbook.BuiltInDocumentProperties.Company);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


