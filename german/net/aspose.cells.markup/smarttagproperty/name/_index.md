---
title: "SmartTagProperty.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagProperty property. Gibt den Namen der Eigenschaft zurück und setzt ihn."
type: docs
url: /de/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Liest und legt den Namen der Eigenschaft fest.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;
    using System.Reflection;

    public class SmartTagPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Instanz von SmartTagProperty mittels Reflexion, da der Konstruktor nicht öffentlich ist.
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Name-Eigenschaft festlegen
                property.Name = "Department";

                // Zeige den aktuellen Wert der Name-Eigenschaft an
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Demonstriere das Ändern der Name-Eigenschaft
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Zeige, dass die Eigenschaft gelesen und geändert werden kann
                Console.WriteLine("Name property demonstration completed successfully");
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


