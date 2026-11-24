---
title: "Klasse CustomProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Properties.CustomProperty-Klasse. Stellt eine benutzerdefinierte Eigenschaft dar, die Namens‑ und Wertepaare beliebiger, vom Benutzer definierter Daten für ein Arbeitsblatt speichert."
type: docs
url: /de/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Stellt eine benutzerdefinierte Eigenschaft dar, die Namens‑ und Wertepaare beliebiger benutzerdefinierter Daten für das Arbeitsblatt speichert.

```csharp
public class CustomProperty
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Liest und setzt den Binärwert der benutzerdefinierten Eigenschaft. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Gibt den Namen des Objekts zurück oder setzt ihn. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Gibt den Wert der benutzerdefinierten Eigenschaft zurück oder setzt ihn. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Gibt den Wert der benutzerdefinierten Eigenschaft zurück oder setzt ihn. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Greife auf die CustomProperties‑Sammlung zu.
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Benutzerdefinierte Eigenschaften hinzufügen.
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Greife auf die benutzerdefinierten Eigenschaften zu und zeige sie an.
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


