---
title: "CustomProperty.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomProperty Property. Gibt den Namen des Objekts zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Gibt den Namen des Objekts zurück oder setzt ihn.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie eine benutzerdefinierte Eigenschaft mit einem Namen und einem Wert hinzu
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Rufen Sie die benutzerdefinierte Eigenschaft ab
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Zeigen Sie den aktuellen Wert der Name-Eigenschaft an (Lesevorgang)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Setzen Sie einen neuen Wert für die Name-Eigenschaft
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Speichere die Arbeitsmappe
                workbook.Save("NameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


