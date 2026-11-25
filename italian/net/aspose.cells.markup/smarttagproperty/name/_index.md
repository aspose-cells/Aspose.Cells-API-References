---
title: "SmartTagProperty.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagProperty. Ottiene e imposta il nome della proprietà"
type: docs
url: /it/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Ottiene e imposta il nome della proprietà.

```csharp
public string Name { get; set; }
```

### Esempi

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
                // Crea un'istanza di SmartTagProperty usando la riflessione poiché il costruttore non è pubblico
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Imposta la proprietà Name
                property.Name = "Department";

                // Visualizza il valore corrente della proprietà Name
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Dimostra la modifica della proprietà Name
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Mostra che la proprietà può essere letta e modificata
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

### Vedi anche

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


