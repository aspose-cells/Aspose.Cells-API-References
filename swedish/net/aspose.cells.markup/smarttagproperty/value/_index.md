---
title: "SmartTagProperty.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagProperty‑egenskap. Hämtar och anger värdet på egenskapen"
type: docs
url: /sv/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Hämtar och sätter värdet på egenskapen.

```csharp
public string Value { get; set; }
```

### Exempel

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
                // Skapa en instans av SmartTagProperty med den icke‑publika konstruktorn
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Ange namn och värde för egenskapen
                property.Name = "Category";
                property.Value = "Finance";

                // Visa egenskapsvärdena
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

### Se även

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


