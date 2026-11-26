---
title: "EquationNode.RemoveChild"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Elimina el nodo especificado de los hijos del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/removechild/
---
## RemoveChild(EquationNode) {#removechild}

Elimina el nodo especificado de los hijos del nodo actual.

```csharp
public void RemoveChild(EquationNode node)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nodo | EquationNode | Nodo a eliminar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveChildWithEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear un nodo de ecuación padre
                EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

                // Agregar dos nodos hijos
                EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
                EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);

                // Verificar que existan los hijos
                Console.WriteLine($"Parent has {(parentNode.GetChild(0) != null ? "first" : "no first")} child");
                Console.WriteLine($"Parent has {(parentNode.GetChild(1) != null ? "second" : "no second")} child");

                // Eliminar el segundo nodo hijo por referencia
                parentNode.RemoveChild(child2);

                Console.WriteLine("Second child node removed successfully");

                // Verificar la eliminación
                Console.WriteLine($"Parent now has {(parentNode.GetChild(0) != null ? "first" : "no first")} child");
                Console.WriteLine($"Parent now has {(parentNode.GetChild(1) != null ? "second" : "no second")} child");

                workbook.Save("EquationNodeRemoveChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## RemoveChild(int) {#removechild_1}

Elimina el nodo en el índice especificado de los hijos del nodo actual.

```csharp
public void RemoveChild(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | Índice del nodo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveChildWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un nodo de ecuación padre
            EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            
            // Agregar nodos hijos
            EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
            EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);
            EquationNode child3 = parentNode.AddChild(EquationNodeType.Matrix);

            try
            {
                // Eliminar el hijo en el índice 1 (segundo hijo)
                parentNode.RemoveChild(1);
                
                Console.WriteLine("Child at index 1 removed successfully");
                
                // Verificar la eliminación comprobando los hijos restantes
                EquationNode remainingChild = parentNode.GetChild(0);
                Console.WriteLine($"First remaining child type: {remainingChild.EquationType}");
                
                // Intentar obtener el hijo eliminado (debería lanzar una excepción)
                try
                {
                    var removedChild = parentNode.GetChild(1);
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Expected error when accessing removed child: {ex.Message}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveChild method: {ex.Message}");
            }
            
            workbook.Save("EquationNodeRemoveChildWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


