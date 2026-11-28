---
title: "MathematicalEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MathematicalEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğümle eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Karşılaştırma için iki MathematicalEquationNode örneği oluşturun.
                // MathematicalEquationNode parametresiz bir yapıcıya sahip olmadığından,
                // null veya uygun parametreler geçmemiz gerekecek
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Düğümleri Equals yöntemiyle karşılaştırın
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Farklı bir nesne türüyle karşılaştırın
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
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

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


