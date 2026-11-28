---
title: "SmartTagProperty.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagProperty özelliği. Özelliğin adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Özelliğin adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

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
                // Kurucu metodunun erişilebilir olmaması nedeniyle yansıma kullanarak SmartTagProperty örneği oluştur
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Name özelliğini ayarlayın
                property.Name = "Department";

                // Name özelliğinin mevcut değerini göster
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Name özelliğini değiştirmeyi gösterin
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Özelliğin okunabileceğini ve değiştirilebileceğini gösterin
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

### Ayrıca Bakınız

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


