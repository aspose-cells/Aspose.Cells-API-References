---
title: "DocumentProperty.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Eigenschaft. Gibt den Datentyp der Eigenschaft zurück"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Ermittelt den Datentyp der Eigenschaft.

```csharp
public PropertyType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf benutzerdefinierte Dokumenteigenschaften (nicht integriert)
            CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Benutzerdefinierte Eigenschaften mit verschiedenen Typen hinzufügen
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 5);
            properties.Add("IsApproved", true);
            
            // Demonstriere die Verwendung der Type‑Eigenschaft
            Console.WriteLine("Document Properties and Their Types:");
            foreach (DocumentProperty prop in properties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
            }
            
            // Auf eine bestimmte Eigenschaft zugreifen und ihren Typ prüfen
            DocumentProperty dateProp = properties["CreatedDate"];
            if (dateProp.Type == PropertyType.DateTime)
            {
                Console.WriteLine("\nCreatedDate is a DateTime property");
                Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
            }
        }
    }
}
```

### Siehe auch

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


