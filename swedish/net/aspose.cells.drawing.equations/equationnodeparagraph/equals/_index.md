---
title: "EquationNodeParagraph.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNodeParagraph‑metod. Avgör om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

Bestäm om den aktuella ekvationsnoden är lika med den angivna noden

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Den angivna noden |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två EquationNodeParagraph‑instanser för jämförelse
            // Använd CreateNode‑metoden för att korrekt instansiera noderna
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // Ställ in olika justeringstyper för att göra dem olika
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // Anropa Equals‑metoden med paragraph2 som parameter
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // Visa jämförelsens resultat
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // Skapa ett annat stycke med samma justering som paragraph1
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // Anropa Equals igen med paragraph3
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // Visa också jämförelse med null
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Spara arbetsboken (även om inga synliga ändringar gjordes i kalkylbladet)
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


