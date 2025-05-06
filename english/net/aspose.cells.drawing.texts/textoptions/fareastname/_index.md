---
title: TextOptions.FarEastName
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Gets and sets the FarEast name
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Gets and sets the FarEast name.

```csharp
public string FarEastName { get; set; }
```

### Examples

```csharp
// Called: shape.TextOptions.FarEastName = &amp;quot;宋体&amp;quot;;
[Test]
        public void Property_FarEastName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46058.xlsx&quot;);
            Shape shape = workbook.Worksheets[0].Shapes[0];

            shape.TextOptions.FarEastName = &quot;宋体&quot;;
            workbook.Save(Constants.destPath + &quot;CellsNet46058.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46058.xlsx&quot;);
            shape = workbook.Worksheets[0].Shapes[0];
            Assert.AreEqual(shape.TextOptions.FarEastName, &quot;宋体&quot;);
        }
```

### See Also

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


