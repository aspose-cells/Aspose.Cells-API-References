---
title: "EquationNode.AddChild"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode‑metod. Infoga en nod av den angivna typen i slutet av den aktuella nodens lista med barnnoder"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | EquationNodeType | Typer av Equation‑noder |

### Returvärde

Om den angivna typen finns returneras den motsvarande noden, och om typen inte finns returneras en nod av okänd typ.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta rot‑matematiknod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa en funktionsnod och lägg till barn
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
            
            // Lägg till funktionsnamn med upphöjt tecken
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
            
            // Lägg till bastext för funktionsnamn
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";
            
            // Lägg till upphöjd text
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";
            
            // Lägg till funktionsargument
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // Spara arbetsboken
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### Se även

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder.

```csharp
public void AddChild(EquationNode node)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| node | EquationNode | Den angivna noden |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en ekvationsform
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Skapa en textnod som fungerar som förälder
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // Skapa en barnnod att lägga till med den statiska metoden CreateNode
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // Anropa AddChild‑metoden med EquationNode‑parameter
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // Spara arbetsboken
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

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


