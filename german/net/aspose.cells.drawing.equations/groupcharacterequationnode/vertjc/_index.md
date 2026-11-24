---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GroupCharacterEquationNode‑Eigenschaft. Dieses Attribut in Kombination mit pos von groupChrPr legt das vertikale Layout des groupChr‑Objekts fest. Dabei gibt pos die Position des Gruppierungszeichens an, vertJc gibt die Ausrichtung des Objekts relativ zur Grundlinie an."
type: docs
url: /de/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Dieses Attribut, kombiniert mit pos von groupChrPr, legt das vertikale Layout des groupChr-Objekts fest. Während pos die Position des Gruppierungszeichens angibt, gibt vertJc die Ausrichtung des Objekts relativ zur Grundlinie an.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Textfeld-Shape, das die Gleichung enthält
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Erstelle eine Instanz von GroupCharacterEquationNode
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Setze die Anfangseigenschaften für den Gleichungsknoten
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // Demonstriere die VertJc‑Eigenschaft (Lesen und Schreiben)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // Ändere den VertJc‑Wert
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Speichere die Arbeitsmappe
                workbook.Save("VertJcDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


