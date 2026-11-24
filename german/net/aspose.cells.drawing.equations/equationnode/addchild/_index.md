---
title: "EquationNode.AddChild"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Fügt einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Fügen Sie einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | EquationNodeType | Typen von Gleichungsknoten |

### Rückgabewert

Wenn der angegebene Typ existiert, wird der entsprechende Knoten zurückgegeben; existiert der Typ nicht, wird ein Knoten unbekannten Typs zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie dem ersten Arbeitsblatt eine Gleichungsform hinzu.
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Den Wurzel-Matheknoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Einen Funktionsknoten erstellen und Kinder hinzufügen
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
            
            // Funktionsnamen mit Hochstellung hinzufügen
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
            
            // Basistext für Funktionsnamen hinzufügen
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";
            
            // Hochstellungstext hinzufügen
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";
            
            // Funktionsargument hinzufügen
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // Speichere die Arbeitsmappe
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein.

```csharp
public void AddChild(EquationNode node)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| node | EquationNode | Der angegebene Knoten |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Gleichungsform erstellen
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Einen Textknoten erstellen, der als Elternteil dient
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // Einen Kindknoten erstellen, der mit der statischen Methode CreateNode hinzugefügt wird
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // AddChild-Methode mit EquationNode-Parameter aufrufen
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // Speichere die Arbeitsmappe
                workbook.Save("EquationNodeAddChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling AddChild: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


