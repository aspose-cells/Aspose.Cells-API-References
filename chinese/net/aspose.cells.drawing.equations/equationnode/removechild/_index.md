---
title: "EquationNode.RemoveChild"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNode 方法。将指定节点从当前节点的子节点中移除"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/removechild/
---
## RemoveChild(EquationNode) {#removechild}

从当前节点的子节点中移除指定的节点。

```csharp
public void RemoveChild(EquationNode node)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 节点 | EquationNode | 待删除的节点。 |

### 示例

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
                // 创建父方程节点
                EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

                // 添加两个子节点
                EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
                EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);

                // 验证子节点是否存在
                Console.WriteLine($"Parent has {(parentNode.GetChild(0) != null ? "first" : "no first")} child");
                Console.WriteLine($"Parent has {(parentNode.GetChild(1) != null ? "second" : "no second")} child");

                // 通过引用移除第二个子节点
                parentNode.RemoveChild(child2);

                Console.WriteLine("Second child node removed successfully");

                // 验证删除
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

### 另请参见

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## RemoveChild(int) {#removechild_1}

从当前节点的子节点中移除指定索引处的节点。

```csharp
public void RemoveChild(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 节点的索引 |

### 示例

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

            // 创建父方程节点
            EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            
            // 添加子节点
            EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
            EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);
            EquationNode child3 = parentNode.AddChild(EquationNodeType.Matrix);

            try
            {
                // 删除索引为 1 的子节点（第二个子节点）
                parentNode.RemoveChild(1);
                
                Console.WriteLine("Child at index 1 removed successfully");
                
                // 通过检查剩余子节点验证删除
                EquationNode remainingChild = parentNode.GetChild(0);
                Console.WriteLine($"First remaining child type: {remainingChild.EquationType}");
                
                // 尝试获取已删除的子节点（应抛出异常）
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

### 另请参见

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


