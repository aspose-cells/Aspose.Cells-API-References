---
title: SaveOptions.UpdateSmartArt
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether updating smart art setting. The default value is false
type: docs
url: /net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

Indicates whether updating smart art setting. The default value is false.

```csharp
public bool UpdateSmartArt { get; set; }
```

### Remarks

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### Examples

```csharp
// Called: options.UpdateSmartArt = (true);
[Test]
        public void Property_UpdateSmartArt()
        {

            Workbook wb = new Workbook(Constants.sourcePath + &quot;JAVA43253.xls&quot;);
            replaceShapeTexts(wb, null);
            XlsSaveOptions options = new XlsSaveOptions();
            options.UpdateSmartArt = (true);
            wb.Save(Constants.destPath + &quot;JAVA43253.xls&quot;, options);
            wb = new Workbook(Constants.destPath + &quot;JAVA43253.xls&quot;);

            Worksheet worksheet = wb.Worksheets[0];
            bool flag = true;
            // 図形
            ShapeCollection shapes = worksheet.Shapes;
            int shapeCount = shapes.Count;
            for (int i = 0; i &lt; shapeCount; i++)
            {
                Shape shape = shapes[i];
                if (shape != null &amp;&amp; shape.IsSmartArt)
                {
                    GroupShape groupShape = shape.GetResultOfSmartArt();
                    Shape[] groupedShapes = groupShape.GetGroupedShapes();
                    foreach (Shape smartart in groupedShapes)
                    {
                        if (!string.IsNullOrEmpty(smartart.Text))
                        {
                            Assert.AreEqual(&quot;test&quot;, smartart.Text);
                        }
                    }
                }
            }
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


