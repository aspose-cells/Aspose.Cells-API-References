---
title: "EquationNodeParagraph.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNodeParagraph‑Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Der angegebene Knoten |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei EquationNodeParagraph‑Instanzen zum Vergleich
            // Verwende die CreateNode‑Methode, um die Knoten korrekt zu instanziieren
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // Setze verschiedene Ausrichtungstypen, um sie ungleich zu machen
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // Rufe die Equals‑Methode mit paragraph2 als Parameter auf
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // Anzeige des Vergleichsergebnisses
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // Erstelle einen weiteren Absatz mit derselben Ausrichtung wie paragraph1
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // Rufe Equals erneut mit paragraph3 auf
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // Zeige außerdem den Vergleich mit null
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe (obwohl keine sichtbaren Änderungen am Arbeitsblatt vorgenommen wurden)
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


