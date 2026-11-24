---
title: "Workbook.CustomDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt eine DocumentProperty-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften des Tabellenblatts darstellt"
type: docs
url: /de/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Gibt eine [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/)‑Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Benutzerdefinierte Dokumenteigenschaften hinzufügen
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Greife auf die benutzerdefinierten Eigenschaften zu und zeige sie an
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


