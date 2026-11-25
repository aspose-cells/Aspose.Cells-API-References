---
title: "ContentTypeProperty.IsNillable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ContentTypeProperty. Indica se il valore può essere vuoto"
type: docs
url: /it/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indica se il valore può essere vuoto.

```csharp
public bool IsNillable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Aggiungi una proprietà di tipo contenuto
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Accedi alla proprietà e imposta IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // Verifica e visualizza il valore di IsNillable
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


