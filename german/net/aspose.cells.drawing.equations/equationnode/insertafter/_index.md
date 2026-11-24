---
title: "EquationNode.InsertAfter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Fügt den angegebenen Knoten nach dem aktuellen Knoten ein"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Fügt den angegebenen Knoten nach dem aktuellen Knoten ein.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
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

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Gleichungsform in Zelle A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Fügen Sie einen initialen Textknoten hinzu
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Fügen Sie einen neuen Textknoten nach dem vorhandenen ein
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Zeigen Sie die Gleichungsstruktur an
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Speichern Sie die Gleichung in einer Zelle zur visuellen Überprüfung
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


