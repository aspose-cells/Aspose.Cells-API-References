---
title: "Clase LimLowUppEquationNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Equations.LimLowUppEquationNode. Esta clase especifica la función límite"
type: docs
url: /es/net/aspose.cells.drawing.equations/limlowuppequationnode/
---
## LimLowUppEquationNode class

Esta clase especifica la función límite.

```csharp
public class LimLowUppEquationNode : EquationNode
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Obtener el tipo de ecuación del nodo actual (Heredado de [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
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
| override [Equals](../../aspose.cells.drawing.equations/limlowuppequationnode/equals/)(object) | Determinar si el nodo de ecuación actual es igual al nodo especificado |
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassLimLowUppEquationNodeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear una instancia de la clase LimLowUppEquationNode
                // Dado que la clase no tiene un constructor público sin parámetros,
                // usaremos un enfoque diferente para demostrar la funcionalidad
                LimLowUppEquationNode limNode = null;
                LimLowUppEquationNode anotherNode = null;

                // Demostrar funcionalidad básica - comprobar igualdad de objetos
                bool areEqual = limNode?.Equals((object)anotherNode) ?? false;

                Console.WriteLine($"LimLowUppEquationNode demonstration");
                Console.WriteLine($"Nodes are equal: {areEqual}");

                // Guarda el libro de trabajo
                workbook.Save("LimLowUppEquationNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LimLowUppEquationNode: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


