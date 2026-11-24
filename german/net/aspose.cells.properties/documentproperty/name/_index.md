---
title: "DocumentProperty.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Eigenschaft. Gibt den Namen der Eigenschaft zurück"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

Gibt den Namen der Eigenschaft zurück.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
            CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
            
            // Füge eine benutzerdefinierte Eigenschaft hinzu und zeige die Verwendung von Name
            DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
            Console.WriteLine("Property Name: " + authorProperty.Name);
            Console.WriteLine("Property Value: " + authorProperty.Value);
            
            // Zugriff auf eine integrierte Eigenschaft über den Namen
            DocumentProperty titleProperty = builtInProps["Title"];
            titleProperty.Value = "Sample Document";
            Console.WriteLine("Title Property Name: " + titleProperty.Name);
            Console.WriteLine("Title Property Value: " + titleProperty.Value);
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


