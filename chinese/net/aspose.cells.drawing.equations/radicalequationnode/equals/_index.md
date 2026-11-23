---
title: "RadicalEquationNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RadicalEquationNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/radicalequationnode/equals/
---
## RadicalEquationNode.Equals method

确定当前方程节点是否等于指定节点

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 指定的节点 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class RadicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // 创建两个 RadicalEquationNode 实例
                RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
                RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));

                // 设置不同的属性以演示相等性比较
                node1.IsDegHide = true;
                node2.IsDegHide = false;

                // 使用 Equals 方法比较节点
                bool areEqual = node1.Equals(node2);

                // 显示比较结果
                Console.WriteLine($"Are nodes equal? {areEqual}");

                // 与相同对象进行比较
                areEqual = node1.Equals(node1);
                Console.WriteLine($"Are node1 and itself equal? {areEqual}");

                // 与 null 比较
                areEqual = node1.Equals(null);
                Console.WriteLine($"Are node1 and null equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


