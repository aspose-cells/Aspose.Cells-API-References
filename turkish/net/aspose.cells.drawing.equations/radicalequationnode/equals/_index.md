---
title: "RadicalEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RadicalEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğümle eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/radicalequationnode/equals/
---
## RadicalEquationNode.Equals method

Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Belirtilen düğüm |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class RadicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // İki RadicalEquationNode örneği oluşturun
                RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
                RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));

                // Eşitlik karşılaştırmasını göstermek için farklı özellikler ayarlayın
                node1.IsDegHide = true;
                node2.IsDegHide = false;

                // Düğümleri Equals yöntemiyle karşılaştırın
                bool areEqual = node1.Equals(node2);

                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"Are nodes equal? {areEqual}");

                // Aynı nesneyle karşılaştırın
                areEqual = node1.Equals(node1);
                Console.WriteLine($"Are node1 and itself equal? {areEqual}");

                // null ile karşılaştır
                areEqual = node1.Equals(null);
                Console.WriteLine($"Are node1 and null equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


