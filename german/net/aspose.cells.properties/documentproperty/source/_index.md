---
title: "DocumentProperty.Source"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Eigenschaft. Die verknüpfte Inhaltsquelle"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

Die verknüpfte Inhaltsquelle.

```csharp
public string Source { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf benutzerdefinierte Dokumenteigenschaften
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Eigenschaften hinzufügen
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Eigenschaften abrufen und ihre Quellen anzeigen
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


