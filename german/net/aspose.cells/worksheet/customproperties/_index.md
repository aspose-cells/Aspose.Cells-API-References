---
title: "Worksheet.CustomProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt ein Objekt zurück, das die mit einem Arbeitsblatt verknüpften Identifikationsinformationen darstellt"
type: docs
url: /de/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Liest ein Objekt, das die Identifikationsinformationen eines Arbeitsblatts darstellt.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Hinweise

Worksheet.CustomProperties bietet einen bevorzugten Mechanismus zum Speichern beliebiger Daten. Es unterstützt Legacy‑Drittanbieter‑Dokumentkomponenten sowie Situationen, die einen strengen Bedarf an Binärteilen haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benutzerdefinierte Eigenschaften zum Arbeitsblatt hinzufügen
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Anzahl der benutzerdefinierten Eigenschaften anzeigen
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Auf Eigenschaftswerte zugreifen und sie anzeigen
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


