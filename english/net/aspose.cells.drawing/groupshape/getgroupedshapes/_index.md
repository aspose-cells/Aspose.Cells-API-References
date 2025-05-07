---
title: GroupShape.GetGroupedShapes
second_title: Aspose.Cells for .NET API Reference
description: GroupShape method. Gets the shapes grouped by this shape
type: docs
url: /net/aspose.cells.drawing/groupshape/getgroupedshapes/
---
## GroupShape.GetGroupedShapes method

Gets the shapes grouped by this shape.

```csharp
public Shape[] GetGroupedShapes()
```

### Examples

```csharp
// Called: Shape[] children = groupShape.GetGroupedShapes();
[Test]
        public void Method_GetGroupedShapes()
        {
            var workbook = new Workbook(Constants.sourcePath + "CellsNet45755.xlsx");
            Worksheet ws = workbook.Worksheets[0];

            int cnt = ws.Shapes.Count;

            for (int i = 0; i < cnt; i++)
            {
                Shape o = ws.Shapes[i];
                if (o.IsSmartArt)
                {
                    GroupShape groupShape = o.GetResultOfSmartArt();
                    Shape[] children = groupShape.GetGroupedShapes();
                    for (int j = 0; j < children.Length; j++)
                    {
                        Console.WriteLine(children[j].Text);
                    }
                }
                else
                {
                    Console.WriteLine(o.Text);
                }

            }

        }
```

### See Also

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


