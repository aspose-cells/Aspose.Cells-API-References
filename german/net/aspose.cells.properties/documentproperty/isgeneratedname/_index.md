---
title: "DocumentProperty.IsGeneratedName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Eigenschaft. Gibt true zurück, wenn diese Eigenschaft keinen Namen im OLE2-Speicher hat und ein eindeutiger Name nur für die öffentliche API generiert wurde"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Gibt true zurück, wenn diese Eigenschaft keinen Namen im OLE2‑Speicher hat und ein eindeutiger Name ausschließlich für die öffentliche API erzeugt wurde.

```csharp
public bool IsGeneratedName { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Greife auf benutzerdefinierte Dokumenteigenschaften zu, um sie hinzuzufügen
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Eine benutzerdefinierte Eigenschaft hinzufügen
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Zeige IsGeneratedName für integrierte Eigenschaft an
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Zeige IsGeneratedName für benutzerdefinierte Eigenschaft an
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Erstelle ein Szenario, in dem eine Eigenschaft einen generierten Namen haben könnte
            // (Hinweis: In der Praxis ist IsGeneratedName schreibgeschützt und wird intern von Aspose.Cells gesetzt)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


