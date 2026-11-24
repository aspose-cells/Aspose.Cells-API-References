---
title: "EquationNode.InsertChild"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in die Kindknotenliste des aktuellen Knotens ein"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in die Kindknotenliste des aktuellen Knotens ein.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Indexwert |
| equationType | EquationNodeType | Typen von Gleichungsknoten |

### Rückgabewert

Wenn der angegebene Typ existiert, wird der entsprechende Knoten zurückgegeben; existiert der Typ nicht, wird ein Knoten unbekannten Typs zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Gleichungsform erstellen
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Initialen Textknoten zur Gleichung hinzufügen
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Einen neuen Bruchknoten an Index 0 einfügen
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Speichere die Arbeitsmappe
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


