---
title: "SmartTagProperty.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagProperty özelliği. Özelliğin değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Özelliğin değerini alır ve ayarlar.

```csharp
public string Value { get; set; }
```

### Örnekler

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
                // SmartTagProperty'nin non‑public yapıcı kullanılarak bir örneğini oluşturun
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Özelliğin adını ve değerini ayarlayın
                property.Name = "Category";
                property.Value = "Finance";

                // Özellik değerlerini göster
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

### Ayrıca Bakınız

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


