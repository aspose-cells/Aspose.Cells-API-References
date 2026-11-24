---
title: "SmartTagProperty.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagProperty property. Gibt den Wert der Eigenschaft zurück und setzt ihn."
type: docs
url: /de/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Liest und legt den Wert der Eigenschaft fest.

```csharp
public string Value { get; set; }
```

### Beispiele

```csharp
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Instanz von SmartTagProperty mit dem nicht‑öffentlichen Konstruktor
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Setze den Namen und den Wert der Eigenschaft
                property.Name = "Category";
                property.Value = "Finance";

                // Zeige die Eigenschaftswerte an
                Console.WriteLine($"SmartTagProperty Name : {property.Name}");
                Console.WriteLine($"SmartTagProperty Value: {property.Value}");
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

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


