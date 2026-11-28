---
title: "BorderBoxEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BorderBoxEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğümle eşit olup olmadığını belirle"
type: docs
url: /tr/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Karşılaştırma için iki BorderBoxEquationNode örneği oluşturun
                // BorderBoxEquationNode parametresiz bir yapıcıya sahip olmadığından,
                // temel sınıf yapıcısını kullanacağız (EquationNode'un bir yapıcıya sahip olabileceğini varsayarak)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Düğümleri Equals yöntemiyle karşılaştırın
                bool areEqual = node1.Equals((object)node2);
                
                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Farklı bir nesne türüyle karşılaştırın
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


