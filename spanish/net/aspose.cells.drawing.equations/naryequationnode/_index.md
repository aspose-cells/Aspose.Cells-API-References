---
title: "Class NaryEquationNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode class. Esta clase especifica una ecuación de operador n-ario que consiste en un operador n-ario, una base o operando y límites superior e inferior opcionales"
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

Esta clase especifica una ecuación de operador n-ario que consiste en un operador n-ario, una base (u operando) y límites superior e inferior opcionales.

```csharp
public class NaryEquationNode : EquationNode
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | Si se muestra el límite inferior |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | Si se muestra el límite superior |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | Este atributo especifica la ubicación de los límites en operadores n-arios. Los límites pueden estar centrados arriba y abajo del operador n-ario, o posicionados justo a la derecha del operador. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con la altura de su operando. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | un operador n-ario, p.\u202fej. "∑". Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador n-ario. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | un operador n-ario, p.\u202fej. "∑" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Especifica el nodo padre del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representa el tipo del nodo. (Heredado de [`EquationNode`](../equationnode/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. (Heredado de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insertar un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
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
    public class EquationsClassNaryEquationNodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el nodo de ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crear un nodo de ecuación n-ario
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Establecer propiedades n-arias
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // Agregar componente base
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // Guarda el libro de trabajo
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### Ver también

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


