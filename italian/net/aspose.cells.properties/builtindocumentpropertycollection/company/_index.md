---
title: "BuiltInDocumentPropertyCollection.Company"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta la proprietà company"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/company/
---
## BuiltInDocumentPropertyCollection.Company property

Ottiene o imposta la proprietà azienda.

```csharp
public string Company { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCompanyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta le proprietà integrate del documento includendo Company
            workbook.BuiltInDocumentProperties.Title = "Annual Report";
            workbook.BuiltInDocumentProperties.Company = "Contoso Ltd";
            
            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx");
            
            // Visualizza le proprietà impostate
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties.Title);
            Console.WriteLine("Company: " + workbook.BuiltInDocumentProperties.Company);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


