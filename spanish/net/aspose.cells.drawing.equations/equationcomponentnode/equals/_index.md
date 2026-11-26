---
title: "EquationComponentNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationComponentNode. Determinar si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationcomponentnode/equals/
---
## EquationComponentNode.Equals method

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

    public class EquationComponentNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //prueba obtener mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            //prueba insertar Fraction
            FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            node.FractionType = EquationFractionType.Skewed;

            string str1 = "A";
            EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
            TR.Text = str1;

            string str2 = "B";
            EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
            TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
            TR.Text = str2;

            // Comparar los nodos usando el método Equals
            bool areEqual = numerator?.Equals((object)denominator) ?? false;

            // Mostrar el resultado de la comparación
            Console.WriteLine($"Nodes are equal: {areEqual}");
            workbook.Save("EquationComponentNodeMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationComponentNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


