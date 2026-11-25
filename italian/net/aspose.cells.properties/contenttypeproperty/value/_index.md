---
title: "ContentTypeProperty.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ContentTypeProperty. Restituisce o imposta il valore della proprietà del tipo di contenuto"
type: docs
url: /it/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Restituisce o imposta il valore della proprietà del tipo di contenuto.

```csharp
public string Value { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Aggiungi una proprietà di tipo contenuto
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Accedi e modifica il valore della proprietà
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
            // Salva la cartella di lavoro
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


