---
title: ShapeCollection.AddLinkedPicture
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add a linked picture
type: docs
url: /net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Add a linked picture.

```csharp
public Picture AddLinkedPicture(int upperLeftRow, int upperLeftColumn, int height, int width, 
    string sourceFullName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | The height of the shape. In unit of pixels |
| width | Int32 | The width of the shape. In unit of pixels |
| sourceFullName | String | The path and name of the source file for the linked image |

### Return Value

[`Picture`](../../picture/) Picture object.

### Examples

```csharp
// Called: workbook.Worksheets[0].Shapes.AddLinkedPicture(1, 0, 100, 100, href);
[Test]
        public void Method_String_()
        {
            var workbook = new Aspose.Cells.Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;Convert the excel file containing the picture URL to HTML&quot;);
            string href = &quot;https://cbu01.alicdn.com/img/ibank/2017/006/292/4531292600_818474941.230x230.jpg&quot;;
            workbook.Worksheets[0].Shapes.AddLinkedPicture(1, 0, 100, 100, href);
            Console.WriteLine(DateTime.Now);
            workbook.Save(_destFilesPath + &quot;CellsJava44016.html&quot;);
            string text = File.ReadAllText(_destFilesPath + &quot;CellsJava44016.html&quot;);
            Assert.IsTrue(text.IndexOf(href) != -1);
            Console.WriteLine(DateTime.Now);
        }
```

### See Also

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


