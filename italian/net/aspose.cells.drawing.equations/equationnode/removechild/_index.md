---
title: "EquationNode.RemoveChild"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Rimuove il nodo specificato dai figli del nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/removechild/
---
## RemoveChild(EquationNode) {#removechild}

Rimuove il nodo specificato dai figli del nodo corrente.

```csharp
public void RemoveChild(EquationNode node)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nodo | EquationNode | Nodo da eliminare. |

### Esempi

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
                // Crea un nodo di equazione genitore
                EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

                // Aggiungi due nodi figli
                EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
                EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);

                // Verifica che i figli esistano
                Console.WriteLine($"Parent has {(parentNode.GetChild(0) != null ? "first" : "no first")} child");
                Console.WriteLine($"Parent has {(parentNode.GetChild(1) != null ? "second" : "no second")} child");

                // Rimuovi il secondo nodo figlio per riferimento
                parentNode.RemoveChild(child2);

                Console.WriteLine("Second child node removed successfully");

                // Verifica la rimozione
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

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## RemoveChild(int) {#removechild_1}

Rimuove il nodo all'indice specificato dai figli del nodo corrente.

```csharp
public void RemoveChild(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | Indice del nodo |

### Esempi

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

            // Crea un nodo di equazione genitore
            EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            
            // Aggiungi nodi figli
            EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
            EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);
            EquationNode child3 = parentNode.AddChild(EquationNodeType.Matrix);

            try
            {
                // Rimuovi il figlio all'indice 1 (secondo figlio)
                parentNode.RemoveChild(1);
                
                Console.WriteLine("Child at index 1 removed successfully");
                
                // Verifica la rimozione controllando i figli rimanenti
                EquationNode remainingChild = parentNode.GetChild(0);
                Console.WriteLine($"First remaining child type: {remainingChild.EquationType}");
                
                // Prova a ottenere il figlio rimosso (dovrebbe lanciare)
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

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


