---
title: "SmartTagProperty.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagProperty. Ottiene e imposta il valore della proprietà"
type: docs
url: /it/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Ottiene e imposta il valore della proprietà.

```csharp
public string Value { get; set; }
```

### Esempi

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
                // Crea un'istanza di SmartTagProperty usando il costruttore non pubblico
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Imposta il nome e il valore della proprietà
                property.Name = "Category";
                property.Value = "Finance";

                // Visualizza i valori delle proprietà
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

### Vedi anche

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


