---
title: "FractionEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FractionEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğüme eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // FractionEquationNode'ın parametresiz bir yapıcıya sahip olmaması nedeniyle,
                // Equals yöntemini, API'de başka yerlerden gelmesi muhtemel nesnelerle göstereceğiz
                // Gösterim amacıyla, karşılaştırmak için iki örnek nesnemiz olduğunu varsayacağız
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Nesneleri Equals kullanarak karşılaştırın
                bool areEqual = node1.Equals(node2);

                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // null ile karşılaştır
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Kendisiyle karşılaştır
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // FractionEquationNode örneklerini almayı taklit eden yardımcı yöntem
        // (Gerçek kullanımda, bunlar API'den gelir)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Bu sadece bir yer tutucudur - gerçekte bunları API'den alırsınız
            // Örneğin: worksheet.Equations.AddFractionEquationNode() veya benzeri
            return null; // Actual implementation would depend on API
        }
    }
}
```

### Ayrıca Bakınız

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


