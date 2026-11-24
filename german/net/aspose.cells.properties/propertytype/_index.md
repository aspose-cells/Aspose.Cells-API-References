---
title: "Enum PropertyType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Properties.PropertyType enum. Gibt den Datentyp einer Dokumenteigenschaft an."
type: docs
url: /de/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Gibt den Datentyp einer Dokumenteigenschaft an.

```csharp
public enum PropertyType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Boolean | `0` | Die Eigenschaft ist ein boolescher Wert. |
| DateTime | `1` | Die Eigenschaft ist ein Datum-Uhrzeit-Wert. |
| Double | `2` | Die Eigenschaft ist eine Fließkommazahl. |
| Number | `3` | Die Eigenschaft ist eine Ganzzahl. |
| String | `4` | Die Eigenschaft ist ein Zeichenkettenwert. |
| Blob | `5` | Die Eigenschaft ist ein Byte-Array. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die integrierten Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Einige integrierte Eigenschaften festlegen
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Zugriff auf die benutzerdefinierten Dokumenteigenschaften
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Benutzerdefinierte Eigenschaften verschiedener Typen hinzufügen
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Benutzerdefinierte Eigenschaften abrufen und anzeigen
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


