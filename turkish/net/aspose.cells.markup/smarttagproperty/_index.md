---
title: "Sınıf SmartTagProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.SmartTagProperty sınıfı. Hücre akıllı etiketi özelliğini temsil eder."
type: docs
url: /tr/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Hücre akıllı etiketinin özelliğini temsil eder.

```csharp
public class SmartTagProperty
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Özelliğin adını alır ve ayarlar. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Özelliğin değerini alır ve ayarlar. |

### Örnekler

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
                // Kurucu metodunun erişilebilir olmaması nedeniyle yansıma kullanarak SmartTagProperty örneği oluştur
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Name ve Value özelliklerini ayarla
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Özellik değerlerini göster
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Özellikleri değiştirmeyi göster
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


