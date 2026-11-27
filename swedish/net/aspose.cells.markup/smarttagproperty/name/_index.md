---
title: "SmartTagProperty.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagProperty‑egenskap. Hämtar och anger namnet på egenskapen"
type: docs
url: /sv/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Hämtar och sätter namnet på egenskapen.

```csharp
public string Name { get; set; }
```

### Exempel

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
                // Skapa en instans av SmartTagProperty med hjälp av reflektion eftersom konstruktorn är icke-offentlig
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Ange Name-egenskapen
                property.Name = "Department";

                // Visa det aktuella värdet på Name‑egenskapen
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Demonstrera ändring av Name‑egenskapen
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Visa att egenskapen kan läsas och modifieras
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

### Se även

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


