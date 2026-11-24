---
title: "GroupCharacterEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GroupCharacterEquationNode‑Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht."
type: docs
url: /de/net/aspose.cells.drawing.equations/groupcharacterequationnode/equals/
---
## GroupCharacterEquationNode.Equals method

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

    public class GroupCharacterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei GroupCharacterEquationNode‑Instanzen zum Vergleich
            // Da GroupCharacterEquationNode keinen parameterlosen Konstruktor hat,
            // müssen wir sie über die ShapeCollection des Arbeitsblatts erstellen
            var shape1 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node1 = (GroupCharacterEquationNode)shape1.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node1.GroupChr = "⏟";
            node1.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node1.Position = EquationCharacterPositionType.Bottom;
            node1.VertJc = EquationCharacterPositionType.Bottom;

            var shape2 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node2 = (GroupCharacterEquationNode)shape2.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node2.GroupChr = "⏟";
            node2.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node2.Position = EquationCharacterPositionType.Bottom;
            node2.VertJc = EquationCharacterPositionType.Bottom;

            try
            {
                // Rufe die Equals-Methode mit dem Object-Parameter auf
                bool areEqual = node1.Equals((Object)node2);

                // Anzeige des Vergleichsergebnisses
                Console.WriteLine($"The two GroupCharacterEquationNode instances are equal: {areEqual}");

                // Füge das Ergebnis dem Arbeitsblatt hinzu
                worksheet.Cells["A1"].PutValue("GroupCharacterEquationNode Equals Comparison Result:");
                worksheet.Cells["A2"].PutValue(areEqual);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("GroupCharacterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


