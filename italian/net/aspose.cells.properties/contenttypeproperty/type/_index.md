---
title: "ContentTypeProperty.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ContentTypeProperty. Ottiene e imposta il tipo della proprietà"
type: docs
url: /it/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Ottiene e imposta il tipo della proprietà.

```csharp
public string Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Aggiungi proprietà di tipo contenuto con tipi diversi
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Accedi e visualizza i tipi delle proprietà
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

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


