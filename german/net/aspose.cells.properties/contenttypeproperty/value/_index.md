---
title: "ContentTypeProperty.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ContentTypeProperty-Eigenschaft. Gibt den Wert der Inhaltstyp-Eigenschaft zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Gibt den Wert der Content‑Typ‑Eigenschaft zurück oder setzt ihn.

```csharp
public string Value { get; set; }
```

### Beispiele

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
            
            // Eine Inhaltstyp-Eigenschaft hinzufügen
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Auf den Wert der Eigenschaft zugreifen und ihn ändern
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
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


