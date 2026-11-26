---
title: "Clase GroupCharacterEquationNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.GroupCharacterEquationNode clase. Esta clase especifica la función GroupCharacter que consiste en un carácter dibujado encima o debajo del texto, a menudo con el propósito de agrupar visualmente los elementos."
type: docs
url: /es/net/aspose.cells.drawing.equations/groupcharacterequationnode/
---
## GroupCharacterEquationNode class

Esta clase especifica la función Group-Character, que consiste en un carácter dibujado encima o debajo del texto, a menudo con el propósito de agrupar visualmente los elementos.

```csharp
public class GroupCharacterEquationNode : EquationNode
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ChrType](../../aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/) { get; set; } | Especificar caracteres combinantes por valor de tipo. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [GroupChr](../../aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/) { get; set; } | Especifica un símbolo (predeterminado U+23DF). Se recomienda encarecidamente usar el atributo ChrType para establecer el carácter de acento. Utilice esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Especifica el nodo padre del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Position](../../aspose.cells.drawing.equations/groupcharacterequationnode/position/) { get; set; } | Este atributo especifica la posición del carácter en el objeto |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representa el tipo del nodo. (Heredado de [`EquationNode`](../equationnode/).) |
| [VertJc](../../aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/) { get; set; } | Este atributo, combinado con pos de groupChrPr, especifica la disposición vertical del objeto groupChr. Donde pos indica la posición del carácter de agrupación, vertJc indica la alineación del objeto con respecto a la línea base. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. (Heredado de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insertar un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/groupcharacterequationnode/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
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
    public class EquationsClassGroupCharacterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Obtener el nodo matemático y agregar el carácter de grupo
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupCharNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Configurar las propiedades del carácter de grupo
            groupCharNode.Position = EquationCharacterPositionType.Top;
            groupCharNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
            
            // Agregar texto base
            EquationNode baseNode = groupCharNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";
            
            // Guarda el libro de trabajo
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


