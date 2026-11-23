---
title: "EquationNode.InsertChild"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNode 方法。在当前节点的子节点列表中，在指定的索引位置插入指定类型的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

在当前节点的子节点列表中，在指定的索引位置插入指定类型的节点。

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 索引值 |
| equationType | EquationNodeType | Equation 节点的类型 |

### 返回值

如果指定的类型存在，则返回相应的节点；如果该类型不存在，则返回未知类型的节点。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建方程形状
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // 向方程添加初始文本节点
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // 在索引 0 处插入新的分数节点
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // 保存工作簿
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


