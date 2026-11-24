---
title: "Klasse SmartTagProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.SmartTagProperty Klasse. Stellt die Eigenschaft des Zell‑Smart‑Tags dar."
type: docs
url: /de/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Stellt die Eigenschaft des Zellen‑SmartTags dar.

```csharp
public class SmartTagProperty
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Liest und legt den Namen der Eigenschaft fest. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Liest und legt den Wert der Eigenschaft fest. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Instanz von SmartTagProperty mittels Reflexion, da der Konstruktor nicht öffentlich ist.
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Setze die Eigenschaften Name und Value
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Zeige die Eigenschaftswerte an
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Demonstriere das Ändern der Eigenschaften
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


