---
title: "Clase MatrixEquationNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Equations.MatrixEquationNode. Esta clase especifica la ecuación de matriz que consiste en uno o más elementos dispuestos en una o más filas y una o más columnas"
type: docs
url: /es/net/aspose.cells.drawing.equations/matrixequationnode/
---
## MatrixEquationNode class

Esta clase especifica la ecuación Matrix, que consiste en uno o más elementos dispuestos en una o más filas y una o más columnas.

```csharp
public class MatrixEquationNode : EquationNode
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BaseJc](../../aspose.cells.drawing.equations/matrixequationnode/basejc/) { get; set; } | Este atributo especifica la justificación de la matriz. El texto fuera de la matriz puede alinearse con la parte inferior, superior o el centro de una función de matriz. Por defecto, la matriz asume justificación centrada. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHidePlaceholder](../../aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/) { get; set; } | Este atributo especifica la propiedad Ocultar Marcadores de posición en una matriz. Cuando esta propiedad está activada, los marcadores de posición no aparecen en la matriz. Por defecto, los marcadores de posición sí aparecen de modo que las ubicaciones donde se puede insertar texto sean visibles. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Especifica el nodo padre del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representa el tipo del nodo. (Heredado de [`EquationNode`](../equationnode/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. (Heredado de [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insertar un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual.(Hereda de [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/matrixequationnode/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
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
    public class EquationsClassMatrixEquationNodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar un cuadro de texto con ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el párrafo de la ecuación y agregar un nodo de matriz
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Establecer propiedades de la matriz
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Agregar una matriz 2x2 con unos en la diagonal
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Guarda el libro de trabajo
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);
            Console.WriteLine("Matrix equation created successfully. File saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


