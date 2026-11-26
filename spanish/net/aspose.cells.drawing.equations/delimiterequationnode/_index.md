---
title: "Clase DelimiterEquationNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Equations.DelimiterEquationNode. Esta clase especifica la ecuación de delimitador que consiste en delimitadores de apertura y cierre como paréntesis, llaves, corchetes y barras verticales, y un componente contenido dentro. El delimitador puede tener más de un componente con un carácter separador designado entre cada componente."
type: docs
url: /es/net/aspose.cells.drawing.equations/delimiterequationnode/
---
## DelimiterEquationNode class

Esta clase especifica la ecuación delimitadora, que consta de delimitadores de apertura y cierre (como paréntesis, llaves, corchetes y barras verticales), y un componente contenido en su interior. El delimitador puede tener más de un componente, con un carácter separador designado entre cada componente.

```csharp
public class DelimiterEquationNode : EquationNode
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BeginChar](../../aspose.cells.drawing.equations/delimiterequationnode/beginchar/) { get; set; } | Carácter inicial del delimitador. |
| [DelimiterShape](../../aspose.cells.drawing.equations/delimiterequationnode/delimitershape/) { get; set; } | Especifica la forma de los delimitadores en el objeto delimitador. |
| [EndChar](../../aspose.cells.drawing.equations/delimiterequationnode/endchar/) { get; set; } | Carácter final del delimitador. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [NaryGrow](../../aspose.cells.drawing.equations/delimiterequationnode/narygrow/) { get; set; } | Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula. |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Especifica el nodo padre del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [SeparatorChar](../../aspose.cells.drawing.equations/delimiterequationnode/separatorchar/) { get; set; } | Carácter separador del delimitador. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representa el tipo del nodo. (Heredado de [`EquationNode`](../equationnode/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. (Heredado de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insertar un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/delimiterequationnode/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Devuelve el nodo en el índice especificado entre los hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserta el nodo especificado después del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserta el nodo especificado antes del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserta un nodo del tipo especificado en la posición de índice especificado en la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Se elimina a sí mismo del padre.(Hereda de [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Elimina todos los nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Elimina el nodo especificado de los hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Elimina el nodo en el índice especificado de los hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Establece el estilo WordArt predefinido.(Hereda de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convertir esta ecuación a expresión LaTeX.(Hereda de [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convertir esta ecuación a expresión MathML.(Hereda de [`EquationNode`](../equationnode/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassDelimiterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crear un nodo delimitador con configuraciones personalizadas
            DelimiterEquationNode node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            node.DelimiterShape = EquationDelimiterShapeType.Match;
            node.NaryGrow = false;
            node.SeparatorChar = "!";
            node.BeginChar = "#";
            node.EndChar = "*";

            // Agregar una fracción como contenido base
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            FractionEquationNode fraction = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);

            // Agregar numerador
            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textRun = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textRun.Text = "A";

            // Agregar denominador
            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            textRun = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textRun.Text = "B";

            // Agregar otro nodo base con texto
            baseNode = node.AddChild(EquationNodeType.Base);
            textRun = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textRun.Text = "a";

            // Guarda el libro de trabajo
            workbook.Save("DelimiterEquationNodeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


