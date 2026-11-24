---
title: "ContentTypeProperty.IsNillable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ContentTypeProperty-Eigenschaft. Gibt an, ob der Wert leer sein könnte"
type: docs
url: /de/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Gibt an, ob der Wert leer sein könnte.

```csharp
public bool IsNillable { get; set; }
```

### Beispiele

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
            
            // Eine Inhaltstyp-Eigenschaft hinzufügen
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Greifen Sie auf die Eigenschaft zu und setzen Sie IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // Überprüfen Sie und geben Sie den IsNillable-Wert aus
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


