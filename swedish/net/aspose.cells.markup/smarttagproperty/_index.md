---
title: "Klass SmartTagProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.SmartTagProperty-klass. Representerar egenskapen för cellens smarta tagg"
type: docs
url: /sv/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Representerar egenskapen för cellens smarta tagg.

```csharp
public class SmartTagProperty
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Hämtar och sätter namnet på egenskapen. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Hämtar och sätter värdet på egenskapen. |

### Exempel

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
                // Skapa en instans av SmartTagProperty med hjälp av reflektion eftersom konstruktorn är icke-offentlig
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Sätt Name- och Value-egenskaperna
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Visa egenskapsvärdena
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Demonstrera modifiering av egenskaperna
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

### Se även

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


