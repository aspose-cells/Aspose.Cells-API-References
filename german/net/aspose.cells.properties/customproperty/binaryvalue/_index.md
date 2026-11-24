---
title: "CustomProperty.BinaryValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomProperty-Eigenschaft. Gibt den Binärwert der benutzerdefinierten Eigenschaft zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Liest und setzt den Binärwert der benutzerdefinierten Eigenschaft.

```csharp
public byte[] BinaryValue { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine benutzerdefinierte Eigenschaft mit einem Beispielwert hinzu
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Rufen Sie die benutzerdefinierte Eigenschaft ab
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Zeigen Sie den Namen und den Wert der benutzerdefinierten Eigenschaft an
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // HINWEIS: Die Reflexion für CustomProperty enthält keine BinaryValue-Eigenschaft.
                // Der verfügbare zeichenbasierte Wert wird über die 'Value'-Eigenschaft abgerufen.

                // Arbeitsmappe speichern (optional)
                workbook.Save("BinaryValueDemo.xlsx");
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


