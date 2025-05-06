---
title: OleObject.IsAutoSize
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated
type: docs
url: /net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

```csharp
public bool IsAutoSize { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].OleObjects[0].IsAutoSize = false;
[Test]
        public void Property_IsAutoSize()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45643.xlsx&quot;);
            Assert.IsTrue(workbook.Worksheets[0].OleObjects[0].IsAutoSize);
            workbook.Worksheets[0].OleObjects[0].IsAutoSize = false;
            workbook.Save(Constants.destPath + &quot;CellsNet45643.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet45643.xlsx&quot;);
            Assert.IsFalse(workbook.Worksheets[0].OleObjects[0].IsAutoSize);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


