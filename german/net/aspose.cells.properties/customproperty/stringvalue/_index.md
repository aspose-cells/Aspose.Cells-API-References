---
title: "CustomProperty.StringValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomProperty Property. Gibt den Wert der benutzerdefinierten Property zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Gibt den Wert der benutzerdefinierten Eigenschaft zurück oder setzt ihn.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die CustomProperty.Value-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juni 2010 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie eine benutzerdefinierte Eigenschaft mit einem Zeichenfolgenwert hinzu
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Rufen Sie die benutzerdefinierte Eigenschaft ab
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Zeigen Sie die StringValue-Eigenschaft an (Lesevorgang)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Setzen Sie einen neuen Wert für die StringValue-Eigenschaft
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Speichere die Arbeitsmappe
                workbook.Save("StringValueDemo.xlsx");
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


