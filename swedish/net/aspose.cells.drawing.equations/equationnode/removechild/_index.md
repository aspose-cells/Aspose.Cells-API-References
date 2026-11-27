---
title: "EquationNode.RemoveChild"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode-metod. Tar bort den angivna noden från den aktuella nodens barn"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/removechild/
---
## RemoveChild(EquationNode) {#removechild}

Tar bort den angivna noden från den aktuella nodens barn.

```csharp
public void RemoveChild(EquationNode node)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| node | EquationNode | Nod som ska raderas. |

### Exempel

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
                // Skapa en föräldraekvationsnod
                EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

                // Lägg till två barnnoder
                EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
                EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);

                // Verifiera att barnen finns
                Console.WriteLine($"Parent has {(parentNode.GetChild(0) != null ? "first" : "no first")} child");
                Console.WriteLine($"Parent has {(parentNode.GetChild(1) != null ? "second" : "no second")} child");

                // Ta bort den andra barnnoden genom referens
                parentNode.RemoveChild(child2);

                Console.WriteLine("Second child node removed successfully");

                // Verifiera borttagning
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

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## RemoveChild(int) {#removechild_1}

Tar bort noden på det angivna indexet från den aktuella nodens barn.

```csharp
public void RemoveChild(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Index för noden |

### Exempel

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

            // Skapa en föräldraekvationsnod
            EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            
            // Lägg till barnnoder
            EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
            EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);
            EquationNode child3 = parentNode.AddChild(EquationNodeType.Matrix);

            try
            {
                // Ta bort barn vid index 1 (andra barnet)
                parentNode.RemoveChild(1);
                
                Console.WriteLine("Child at index 1 removed successfully");
                
                // Verifiera borttagning genom att kontrollera återstående barn
                EquationNode remainingChild = parentNode.GetChild(0);
                Console.WriteLine($"First remaining child type: {remainingChild.EquationType}");
                
                // Försök att hämta borttaget barn (ska kasta ett undantag)
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

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


