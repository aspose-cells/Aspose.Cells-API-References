---
title: "AccentEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AccentEquationNode. Determine si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/accentequationnode/equals/
---
## AccentEquationNode.Equals method

Determinar si el nodo de ecuación actual es igual al nodo especificado

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El nodo especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class AccentEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //prueba obtener mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            AccentEquationNode node = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            node.AccentCharacter = "\u0302";

            AccentEquationNode node2 = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            node2.AccentCharacter = "\u0302";

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            TR.Text = "x";

            EquationNode subBase2 = node2.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR2 = (TextRunEquationNode)(subBase2.AddChild(EquationNodeType.Text));
            TR2.Text = "y";
            Console.WriteLine("AccentEquationNode.Equals(Object) method is called: " + node.Equals(node2));

            workbook.Save("AccentEquationNodeMethodEquals.xlsx");
           
        }
    }
}
```

### Ver también

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


