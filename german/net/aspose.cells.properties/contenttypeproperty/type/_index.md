---
title: "ContentTypeProperty.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ContentTypeProperty-Eigenschaft. Ruft den Typ der Eigenschaft ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Liest und setzt den Typ der Eigenschaft.

```csharp
public string Type { get; set; }
```

### Beispiele

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
            
            // Fügen Sie Content-Type-Eigenschaften mit verschiedenen Typen hinzu
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Greifen Sie auf Eigenschaftstypen zu und zeigen Sie sie an
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


